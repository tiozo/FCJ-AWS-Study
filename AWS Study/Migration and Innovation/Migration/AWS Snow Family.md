### Def.

AWS Snow Family is a group of devices that transport data in and out of AWS.
AWS Snow Family devices are physical devices.
Can transfer up to exabytes of data. (1 Exabytes = 1 000 000 000 000 bytes)
AWS Snow Family include three device types: 
- AWS Snowcone
- AWS Snowball
- AWS Snowmobile

### [[AWS Snowcone]]

AWS Snowcone is a secure and small device.
It transfer data.
It made out of 8TB of storage space, 4GB of memory, and 2 CPUs.

### [[AWS Snowball]]

AWS Snowball has 2 types of devices.

| `Snowball Edge Storage Optimized devices`          | `Snowball Edge Compute Optimized devices`                                                                      |
| -------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| Great for large-scale data migrations              | Great for services that require a large amount of computing resources.                                         |
| Have 80 TB of HDD storage space for object storage | Have 42 TB of HDD storage for object storage, and 7.68 TB of NVMe SSD storage space for AWS EBS block volumes. |
| Have 1 TB of SSD storage for block volumes         | Work on 208 Gib of memory and 52 vCPUs.                                                                        |

### [[AWS Snowmobile]]

AWS Snowmobile moves large amount of data to AWS.
It can transfer up to 100 petabytes of data. (1/10 of 1 Exabyte)
