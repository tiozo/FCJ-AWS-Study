### Why EC2 ?
Makes the process of increasing and decreasing capacity better.
Access resources at demand.
No upfront investment.
Pay for what you need.
EC2 is secure.

### EC2 Termination

### What Remains After Termination

- **EBS Volumes (Most of Them)** This is the most critical one.
    - **Data Volumes (non-root):** By default, any _additional_ EBS volumes (e.g., D: or E: drives) you attached to the instance **do not** get deleted. Their `DeleteOnTermination` flag is set to `false` by default. They will become "available" in the EBS console, and you will continue to pay for them.
    - **Root Volume (Conditionally):** The main OS drive (the C: drive or `/dev/sda1`) _is_ deleted by default. However, if you explicitly changed its `DeleteOnTermination` flag to `false` (either at launch or while it was running), it will also persist.
- **EBS Snapshots** Any snapshots (backups) you created from your EBS volumes are completely separate from the instance and **always** remain.
- **Elastic IP Addresses (EIPs)** If you attached an EIP (a static public IP) to your instance, it is **disassociated** but **remains in your account**.
    - **Warning:** AWS starts charging you for unattached EIPs, so you must release it manually if you no longer need it.
        
- **Security Groups** Security Groups are just firewall rules. They are _associated_ with an instance, not part of it. The Security Group itself remains in your account and can be used for other instances.
    
- **AMIs (Amazon Machine Images)** If you created a custom AMI (a template) from your instance, it is stored separately (backed by S3) and is **not** deleted.
    
- **Data in Other Services** Any data the instance was interacting with in other services is completely unaffected. This includes:
    
    - **S3 Buckets**
        
    - **RDS Databases**
        
    - **DynamoDB Tables**
        
    - **EFS File Systems**
        
    - **CloudWatch Logs:** Log groups and log streams created by the instance will persist (and you will be charged for their storage) unless you have a retention policy set to delete them.
        
- **Key Pairs** The public key you specified when launching the instance remains in your AWS account. The private key (`.pem` file) remains on your local machine.
    

---

### What is DELETED (For Contrast)

It's just as important to know what is permanently lost:

- **The Instance Itself:** The compute, CPU, and RAM configuration are gone forever.
    
- **Instance Store Volumes:** Any data on "ephemeral" or "instance store" drives is **permanently wiped**. This type of storage is physically attached to the host machine and is not persistent.
    
- **The Root EBS Volume (By Default):** As mentioned above, the default behavior is to delete the main OS disk.
    
- **Auto-Assigned Public IP:** If you did _not_ use an Elastic IP, the dynamic public IP the instance had is released back into Amazon's pool and is gone.
    
- **All Data in RAM:** Any in-memory data is lost.