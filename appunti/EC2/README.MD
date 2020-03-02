# EC2
**Amazon Elastic Compute Cloud** is just a virtual server in the cloud.
EC2 reduces the time required to obtain and boot new server instances to minute to minutes, allowing you to quickly scale capacity, both up down, as your computing requirements change.

# EC2 Pricing Models:
1. On Demand: allows you to pay a fixed rate by the hour (or by second) with no commitment.
2. Reserved: provides you with a capacity reservation, and offer a significant discount on the hourly charge for an instance. Contract Terms are 1year or 3year.
3. Spot: enables you to bid whatever price you want for instance capacity, providing for even greater savings if your applications have flexible start and end times.
4. Dedicated Hosts: Physical EC2 server dedicated for your use. Dedicated Hosts can help you reduce costs by  allowing you to use your existing server-bound software licenses.


# EBS
Amazon EBS allows you to create storage volumes and attach the to Amazon EC2 instances. Once attached, you can create a file system on top of these volumes, run a database, or use a block device. Amazon EBS volumes are placed in specific AZ, where they are automatically replicated to protect you from the failure of a single component.

# EBS volume types
       -SSD
* General Purpose SSD (GP2): balances price and performance for a wide variety of workloads.
* Provisioned IOPS SSD (IO1): highest-performance SSD volume for mission critical low-latency or high-throughput workloads.

        -Magnetic
* Throughput Optimized HDD (ST1): low cost HDD volume designed for frequently accessed, throughput-intensive workloads.
* Cold HDD (SC1): lowest cost HDD volume designed for less frequently accessed workloads (File Servers).
* Magnetic: previous generation.



EC2 is a compute based service, it is not serverless. It’s a server.
Use a private key to connect to EC2.
Security Groups are virtual firewalls in the cloud. 

## Common Ports:
* Linux = SSH (Port 22)
* Microsoft = RDP (Port 3389)
* HTTP = Port 80;    HTTPS = Port 443.

You can interact with AWS in 3 ways:
* Using te console
* Using the CLI (Command Line Interface)
* Using the SDKs (Software Development Kits)


