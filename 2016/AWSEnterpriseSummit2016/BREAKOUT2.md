## DevOps Automation & Managed Services
>"Put everything possible into a repository!"

##### Speaker: Hubert Cheung
##### Slides: http://www.slideshare.net/AmazonWebServices/devops-on-aws-deep-dive-on-infrastructure-as-code-toronto

### Deep Dive on Infrastructure as Code

- Application configuration
  - Application Configuration -> CodeDeploy
- Operating System and Host configuration
  - AWS Resources + Operating System -> CloudFormation
  - Operating System + Application configuration -> OpsWorks
- AWS Resources
  - AWS Resources + Operating System -> CloudFormation

### CloudFormation
- Template Anatomy:
  - Declarative language
  - JSON, YAML, XML?
  - Blocked out:
    - Headers
    - Parameters
    - Mappings
    - Conditionals
    - Resources
    - Outputs
- cfn**-init**/**-metadata**/**-signal**/**-hup** for executing after the instance is created
- Install packages needed through cfn metadata
- Entire infrastucture can be represented in a CloudFormation template
- Use version control with your template!!
- Build out multiple environments on same template
- CloudTrail works with CloudFormation to track changes/updates
- Template validation: `aws cloudformation validate-tempalte` - confirm CF syntax
- CloudFormation Designer Tool
- Tricky to do at scale for:
  - Changing vhost

### OpsWorks
- Configuration management solution for automating operational tasks
- Model, control and automate applications
- Opsworks is:
  - The **Stack**, cloud infrastructure and applications
  - A **Layer** defines how to setup and configure a set of instances related to a resources
  - Opswork Agents (does all the work)
- Works through an IAM role that passes instance private key, and OpsWork public key
- OpsWorks uses Chef under the hood

### CodeDeploy
- Rolling deploys with zero downtime
- Perform host management as part of a deploys
- Deploy to any instance, AWS or on-premises
- Treat all environments the same
- CodeDeploy Agents (does all the work)
- Uses YAML for application spec
- Hooks used, executes scripts to do things
- Rolling deployment by doing one at a time, half at a time, or all at once
- Uses `aws` cli to do the actual deploys
