### Cloud Storage - [[AWS Simple Storage Service|AWS S3]]

S3 is a storage service.
It allows uploading any type of files.
In S3 you can set access permission a file.
It is object-level storage.

```
Offer unlimited space in storage.
Maximal Object Size is 5TB.
```

### Define Object-Level Storage

Object-Level contains objects.
Each object is made of: 
- Date - any type of files
- Metadata - information about what the data is.
- Key - Unique identifier
![[Pasted image 20251028131435.png]]

### [[AWS S3]] Storage Classes

There are many AWS S3 storage classes.
They differ in data availability
How frequent data is retrieved and cost price.

### S3 Standard

Ideal for data that is accessed often.
Provides high availability for stored objects.
It stores data in at least three AZs.
It is the most expensive class.

### S3 Standard-Infrequent Access - [[S3 Standard-IA]]

S3 standard-ia is ideal for data that is often accessed.
it has the same level of data availability as S3 standard.
It stores data in at least 3 AZs.
Lower storage price but higher data retrieval price.
It is higher priced than other classes.

### [[S3 Inteligent-Tiering]]

Requires automation and monitoring.
Ideal for data with unknown or frequently changing access.
It moves the object to the S3 Standard-IA class if it is not accessed for 30 days.
It moves object to S3 Standard if accessed in S3 Standard-IA or S3 One Zone-IA classes.

