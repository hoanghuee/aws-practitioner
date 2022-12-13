##IAM Section: Identity and Access Management
- IAM is a global service, different from EC2 is a regional service

(An IAM entity that defines a set of permissions for making AWS service requests, that will be used by AWS services)

###1. Users & Groups:
- Root account: created by default and can not use or share
- Users: one user is one people and can be grouped to manage
- Groups: only contain users, not groups
- user can be in 0 or n groups
###2. IAM Permissions:
- User can access AWS with 2 way: root or IAM user
- Policies: define user’s or group‘s permission to some specific service
- Roles: for EC2 instances or AWS services
###3. IAM Policies structures: (ISON document)

→ Ex: Policy: AdministratorAcess

Permission JSON file:
```json
{
    "statement" : [
        {
            "Action": "*",
            "Resource": "*"
        }
    ]
}
```

**Note:**
on-premises:

Phần mềm tại chỗ được cài đặt và chạy trên các máy tính tại cơ sở của cá nhân hoặc tổ chức sử dụng phần mềm, chứ không phải tại một cơ sở từ xa như máy chủ hoặc đám mây.