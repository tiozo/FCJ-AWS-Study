### What are Instance Stores ? 

Instance Store is a storage volume that acts as a physical hard drive.
It provides temporary storage for [[AWS EC2]] instance.
The Data in an instance store persists during the lifetime of its instance.
If an instance reboots, data in instance store will persist.
When the instance hibernates or terminates, you lose any data in the instance store.

```
If an instance starts from a stopped state, it might start on another host where the used instance store does not exist.

It is recommended to avoid storing valuable data in the store instance.

Instance Stores are good for temporary files, and data that can be easily recreated.
```

Examples:
AWS EC2 instance with an attached instance store is running.
![[Pasted image 20251028113529.png]]
AWS EC2 instance is stopped or terminated.
![[Pasted image 20251028113545.png]]
All data on the attached instance store are deleted.
![[Pasted image 20251028113555.png]]
