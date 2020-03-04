# **S3**

**Simple Storage Service** is one of the most fundamental services for AWS. S3 provides developers and IT teams with secure, durable, highly-scalable object storage. 
Amazon S3 is easy to use, with a simple web services interface to store and recovery any amount of data from anywhere on the web.


## **S3 features**
* Easy to use
* Durable (99.99999999999%)
* Available (99.99%)
* High performance
* Scalable
* Secure
* Integration


## **The basics of S3 (Buckets and Objects)**
* S3 is Object-based, so it allows you to upload files
* File can be from 0 Bytes to 5 TB
* There is unlimited storage
* Files are stored in Buckets (are folders in the cloud)
* Bucket name are unique globally and DNS-compliant, must be between 3 and 63 char. long (ex. https://my-s3bucket.s3.amazonaws.com/)
* When you upload a file to S3, you will receive a HTTP 200 code if the upload was successful.

### **S3 is object based. Think of objects just as files. Objects consist of the following:**
* Key name: is the name of the object (alphanumeric characters, special char.)
* Value: is the data and is mad up of a sequence of bytes
* Version ID: important for versioning
* Metadata: data about data you are storing (name + value), there two types:
    * System-defined metadata 
    * User-defined metadata
* Subresources: access Control Lists, Torrent.
### **You can create/access to a bucket with:**
* Amazon S3 Console
* AWS CLI
* SDKs
### **Use cases**
* Backup storage
* Media hosting
* Application assets
* Data lake
* Content delivery
### **How does data consistency work for S3?**
* Read after Write consistency for PUTS of new Objects
* Eventual Consistency for overwrite PUTS and DELETES (can take some time to propagate)


## **S3 Storage Classes**
1. **S3 Standard**: designed for active data and milliseconds access (99.99% availability, 99.99999999999 durability).
2. **S3 Intelligent Tiering**: designed to optimize costs by automatically moving data to the most cost-effective access tier, without performance impact or operational overhead, for active and infrequently accessed data. Initial Intelligent Tiering put data in frequent access tier, after 30 days without access, any objects are move into infrequent access tier.
3. S3 Standard-IA: Infrequently Accessed, for data that is accessed less frequently, but requires rapid access when needed. Lower fee than S3, but you are charged a retrieval fee. 
4. **S3 One Zone-IA**: for where you want a lower-cost option for infrequently accessed data, but do not require the multiple Availability Zone data resilience, your data is stored in only 1 AZ, all other storage classes store data in a least 3 AZ.
5. **S3 Glacier**: is a secure, durable, and low-cost storage class for data archiving, minutes to hours access.
6. **S3 Glacier Deep Archive**: is Amazon S3’s lowest-cost storage class where a retrieval time of 12 hours is acceptable, long-term archive data.


## **Consider:**
* The type of data 
* Resiliency requirements 
* Usage pattern


## **Restricting Bucket Access**
* Bucket Policies - Applies across the whole bucket
* Object Policies - Applies to individual files
* IAM Policies to Users & Groups - Applies to Users & Group

