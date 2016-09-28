## Protecting Your Data in AWS
##### Speaker: Danielle Greshock

- Understand your options for protecting data with encryption in AWS
- Securing acces to data on Amazon S3 using policies
- Database platform security
- Automatically audit and monitor

### Transport security

- TLS to/from AWS API
- Amazon Certificate Manager (ACM)
- Provision trusted SSL/TLS scertificates from AWS
- AWS ACM handles the muck (keypair, CSR generation, renewal)
- Multiple domain certificates
- AWS ACM Only used with ELB, CloudFront
- AWS ACM free.
- s2n library for implementing transport security (Github repo)

### Data at rest security

- Key Questions to consider:
  - Where are keys stored? (My hardware, cloud provider, etc)
  - Where are keys used?
  - Who can use the keys? (Users, applications, etc)
  - What assurances are there for proper security around keys?
- Options:
  - Client Side encryption
  - Server Side encryption
- AWS Key Management Service (*Integrated with CloudTrail!*)
- 
