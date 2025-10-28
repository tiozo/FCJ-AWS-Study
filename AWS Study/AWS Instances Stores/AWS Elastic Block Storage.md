### Def - [[AWS EBS]]

AWS EBS is also called AWS Elastic Block Store.
EBS is a service that provides storage volumes.
You can provided storage volumes in [[AWS EC2]].
EBS volumes are used for data that need to persist.
It is important to backup the data with AWS EBS Snapshots.

```
After creating an EBS volume, you can attach it to an AWS EC2 instance.

If the EC2 instance stops or is terminated, all the data on the attached EBS volume remains.
```

### What are AWS EBS Snapshots ?

EBS Snapshot is an incremental data backup.
The first backup of a volume backups all the data.
Every next backup copies only a block of data that has changed since the last snapshot.
It saves on storage costs by not duplicating data.
![[Pasted image 20251028114635.png]]

```
Only the data unique to that snapshot is removed when you delete a snapshot.

If the EC2 instance stops, or is terminated, all the data on the attached EBS volume remains.
```