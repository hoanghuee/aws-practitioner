## IAM: Password Policy
- Bcus strong password makes higher security for your acc
###1. Password policy such as:
- set min length
- require character types
- allow or not IAM users can change pass
- require IAM user change pass
###2. Using MFA(multi factor auth) = **password + security divide** (you own)
- virtual MFA device as Gg auth
- universal 2bd factor  (U2F) security key (3rd party device) **->allowed by AWS: Gemalto, SurePassID**
- _**Way to access**_: /security_credentials -> manage MFA device

###3 .Access AWS ways (3)
- AWS Management Console
- AWS CLI (Direct access) use cmd in your cmd line
- AWS SDK (for code): embedded within your app

#### AWS Cloud Shell: Region Available

## IAM: Security Tools
###1. Credentials Report (account-level):
- list all status & various credentials of acc’s user (trạng thái của các thông tin đăng nhập khác nhau của account user)
- _**Way to access**_: IAM -> Credentials Report
###2. Access Advisor (user-level):
- show all service permissions granted to user and when last they accessed
- _**Way to access**_: IAM -> Roles -> Access Advisor

##IAM: Shared Responsibility Model
###1. AWS: all infrastructure of AWS
- global network security
- config & vulnerability analysis
- compliance validation

###2. User: users who use infrastructure of AWS
- Create user, gr, role, policy, manage & monitor them
- enable all MFA on all acc
- appreciate & review permission

##IAM Guide
- Dont use the root acc except for AWS account setup
- 1 physical user = 1 aws user => so if a friend wants to use your aws service so create another user for them.
- assign user to groups & permission to groups
- create and use Roles for giving permission to AWS services
- use access key for CLI/SDK
- audit (check) permissions of account with IAM Credentials report (or Access Advisor )
- never share pass & access key

###`Don't give more permissions than the user needs.`

#### 2 way to access AWS with user:
- root user/ user: use email & pass = a physical user
- IAM user: use username & pass created by root user
