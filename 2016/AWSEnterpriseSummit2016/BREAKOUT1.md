## Getting Started with AWS Security - Breakout 1

*This breakout was so goddamn slow and confusing flow what happened to 5,6,7,8?*

##### Speaker: Rahul Sareen

Approach:
 1. Understand AWS Security Practice
 2. Build Strong Compliance Foundations
 3. Integrate Identity & Access management
 4. Enable Detective Controls
 5. Establish Network Security
 6. Implement Data Protection
 7. Optimize Change Management
 8. Automate Security Functions

### 1. Understand AWS Security Practice
 - Traditionally lack of visibility, low degree of automation in enterprise security
 - Promote culture of "everyone is an owner" for security (Distributed & Embedded)
 - Makes security a stakeholder in business success (Distributed & Embedded)
 - Over 30 global compliance certifications and accreditations
 - We're responsible for the security **in** the cloud (*platform, applications, IAM, operating system, network/firewall, client/server side encryption, network traffic protection*), AWS is responsible for the security **of** the cloud (*hardware, patching of the OS*).
 - **Training:** Security Fundamentals on AWS (free online course)
 - **Training:** Security Operations on AWS (3-day class)

### 2. Building Strong Compliance Foundations

- AWS Assurance Programs:
  - SOC 1 Type II
  - SOC 2 Type II and public SOC 3 report
  - ISO 27001, 27017, 27018 certifications
  - Certified PCI DSS Level 1 Service Provider
  - FedRAMP Authorization
  - Architect for HIPAA compliance
- https://aws.amazon.com/security
- AWS Trusted Advisor tool has Cost optimization, Performance, Security, Fault Tolerance

### 3. Integrate Identity & Access Management

- IAM Users
- IAM Groups
- IAM Roles
- IAM Policies
- Account Governance?

### 4. Enable Detective Controls

- AWS CloudTrail
  - Enable Globally for all AWS Regions
  - Encryption & Integrity Validation
  - Archive & Forward
  - Watches user actions within AWS?
- Amazon CloudWatch
  - Amazon CloudWatch Logs
  - Metrics & Filters
  - Alarms & Notifications (*Can create checks when any new instance is created has a valid AMI from a defined list of AMIs*)
  - VPC Flow Logs:
    - Agentless
    Enable per ENI, per subnet, or per VPC
    - Logged to AWS CloudWatch LogsCreate CloudWatch metrics from log Data
    - Alarm on those metrics
    - Can hookup to AWS Elasticsearch service to make graphs/dashboard

Questions:
- Costs associated with CloudTrail and CloudWatch?

### 5. Establish Network Security
- AWS KMS
  - Deep Integration with AWS Services
  - CloudTrail
  - AWS SDK for application encryption
- Amazon CloudHSM (Hardware Security Management)
  - Dedicated HSM
  - Integrate with on-premises HSMS
  - Hybrid architectures
- AWS Config
  - Record configuration changes continuously
  - Time-series view of resource changes
  - Archive & compare
- AWS Config Rules
  - Enforce best practices
  - Automatically rollback unwanted changes
  - Trigger additional workflow
- AWS CloudFormation
  - Infrastructure as code
  - **Miho approved.**


- Assign network Security Group to the Firewall sg-XXXXXX

### 6. Implement Data Protection
### 7. Optimize Change Management
### 8. Automate Security Functions
