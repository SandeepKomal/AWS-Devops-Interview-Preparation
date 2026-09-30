# Amazon S3 Interview Questions

## Fundamentals
1. What is an S3 bucket and object?
2. What are S3 storage classes?
3. How does versioning work?
4. What is a lifecycle policy?
5. What is Object Lock?
6. What is multipart upload?

## Security
Know Block Public Access, IAM policies, bucket policies, Object Ownership, encryption at rest, TLS in transit, VPC endpoints and CloudTrail data events where required.

Do not treat ACLs as the default access-control mechanism for modern designs. Prefer policy-based access and appropriate S3 Object Ownership settings.

## Scenarios
### Private workload must access S3
Explain an S3 VPC endpoint, routing, IAM permissions and bucket-policy conditions.

### Object was accidentally deleted
Explain versioning, recovery of a previous version and controls that reduce recurrence.

### S3 costs increased
Check storage class, object age, retrieval patterns, request volume, incomplete multipart uploads and lifecycle rules.

### Secure static content delivery
Discuss S3 as an origin with CloudFront, TLS, DNS and appropriate access controls.

### Prevent public exposure
Use Block Public Access, least privilege, policy review, monitoring and automated policy checks.
