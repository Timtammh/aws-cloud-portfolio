# 01 — IAM & Security

## AWS Services Used
- AWS IAM (Users, Groups, Roles, Policies)
- AWS Root User
- Multi-Factor Authentication (MFA)

## What I Built
- Created IAM Users and Groups with least-privilege policies
- Configured Role-Based Access for EC2
- Secured Root User with MFA
- Completed Lab 1: Introduction to IAM (Grade: 100%)

## Key Concepts Learned

### Shared Responsibility Model
| AWS Responsible | Customer Responsible |
|----------------|---------------------|
| Physical hardware | IAM Users & permissions |
| Global infrastructure | MFA configuration |
| Hypervisor | Data encryption |
| Managed services | Application security |

### IAM Components
| Component | Purpose |
|-----------|---------|
| User | Individual identity with credentials |
| Group | Collection of users sharing permissions |
| Role | Temporary permissions assumed by services |
| Policy | JSON document defining allowed actions |

### Root User Best Practices
- Never use root for daily tasks
- Enable MFA immediately after account creation
- Create admin IAM user for regular use

## Architecture
![IAM Architecture](./iam-architecture.png)

## Lab Screenshot
![Lab 1 Result](./lab1-result.png)

## Lessons Learned
- IAM Role vs IAM User: Roles are for services/temporary access, Users are for people
- Least privilege principle: only grant permissions actually needed
- MFA adds critical second layer even if password is compromised
