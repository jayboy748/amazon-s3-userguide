--------

Welcome to the new **Amazon S3 User Guide**\! The Amazon S3 User Guide combines information and instructions from the three retired guides: *Amazon S3 Developer Guide*, *Amazon S3 Console User Guide*, and *Amazon S3 Getting Started Guide*\.

--------

# Managing data access with Amazon S3 access points<a name="access-points"></a>

Amazon S3 Access Points simplify managing data access at scale for shared datasets in S3\. Access points are named network endpoints that are attached to buckets that you can use to perform S3 object operations, such as `GetObject` and `PutObject`\. Each access point has distinct permissions and network controls that S3 applies for any request that is made through that access point\. Each access point enforces a customized access point policy that works in conjunction with the bucket policy that is attached to the underlying bucket\. You can configure any access point to accept requests only from a virtual private cloud \(VPC\) to restrict Amazon S3 data access to a private network\. You can also configure custom block public access settings for each access point\.

**Note**  
You can only use access points to perform operations on objects\. You can't use access points to perform other Amazon S3 operations, such as modifying or deleting buckets\. For a complete list of S3 operations that support access points, see [Access point compatibility with S3 operations and AWS services](access-points-usage-examples.md#access-points-service-api-support)\.
Access points work with some, but not all, AWS services and features\. For example, you can't configure Cross\-Region Replication to operate through an access point\. For a complete list of AWS services that are compatible with S3 access points, see [Access point compatibility with S3 operations and AWS services](access-points-usage-examples.md#access-points-service-api-support)\.

This section explains how to work with Amazon S3 access points\. For information about working with buckets, see [Buckets overview](UsingBucket.md)\. For information about working with objects, see [Amazon S3 objects overview](UsingObjects.md)\.

**Topics**
+ [Configuring IAM policies for using access points](access-points-policies.md)
+ [Creating access points](creating-access-points.md)
+ [Using access points](using-access-points.md)
+ [Access points restrictions and limitations](access-points-restrictions-limitations.md)