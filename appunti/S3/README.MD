#S3

**Simple Storage Service** is one of the most fundamental services for AWS. S3 provides developers and IT teams with secure, durable, highly-scalable object storage. 
Amazon S3 is easy to use, with a simple web services interface to store and recovery any amount of data from anywhere on the web.

# The basics of S3
* S3 is Object-based, so it allows you to upload files
* File can be from 0 Bytes to 5 TB
* There is unlimited storage
* Files are stored in Buckets (are folders in the cloud)
* S3 is a universal namespace, the names must be unique globally (ex. https://s3-eu-west-1.amazonaws.com/acloudgiuly)
* When you upload a file to S3, you will receive a HTTP 200 code if the upload was successful.

# S3 is Object based. Think of Objects just as files. Objects consist of the following:
* Key: This is simply the name of the object
* Value: This is simply the data and is mad up of a sequence of bytes
* Version ID: Important for versioning
* Metadata: Data about data you are storing
* Subresources: Access Control Lists, Torrent.

# How does data consistency work for S3?
* Read after Write consistency for PUTS of new Objects
* Eventual Consistency for overwrite PUTS and DELETES (can take some time to propagate)

# S3 features
* Tiered Storage Available
* Lifecycle Management
* Versioning
* Encryption 
* Secure your data using Access Control Lists and Bucket Policies 

# S3 Storage Classes
1. S3 Standard: 99.99% availability, 99.99999999999 durability.
2. S3-IA: Infrequently Accessed, for data that is accessed less frequently, but requires rapid access when needed. Lower fee than S3, but you are charged a retrieval fee.
3. S3 One Zone-IA: for where you want a lower-cost option for infrequently accessed data, but do not require the multiple Availability Zone data resilience.
4. S3-Intelligent Tiering: designed to optimize costs by automatically moving data to the most cost-effective access tier, without performance impact or operational overhead.
5. S3 Glacier: is a secure, durable, and low-cost storage class for data archiving. Retrieval times configurable from minutes to hours.
6. S3 Glacier Deep Archive: is Amazon S3’s lowest-cost storage class where a retrieval time of 12 hours is acceptable.

# Restricting Bucket Access
* Bucket Policies - Applies across the whole bucket
* Object Policies - Applies to individual files
* IAM Policies to Users & Groups - Applies to Users & Group

