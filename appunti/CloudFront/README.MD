# CloudFront
**Amazon CloudFront** can be used to deliver your entire website, including dynamic, static, streaming, and interactive content using a global network of edge locations. Requests for content are automatically routed to nearest edge location.

A CDN (Content Delivery Network) is a system of distributed servers that delivery webpages and other web content to a user based on the geographic locations of the user, the origin of the webpage, and a content delivery server.

## Key Terminology:
* Edge Location: this is the location where content will be cached. They are cached for the life of the TTL (Time To Live) (seconds).
* Origin: this is of all the files that the CDN will distribute. This can be an S3 Bucket, an EC2 Instance, an Elastic Load Balancer, or Route55.
* Distribution: this is the name given the CDN which consists of a collection of Edge Locations.
* Web Distribution: typically used for Websites.
* RTMP: used for Media Streaming.

