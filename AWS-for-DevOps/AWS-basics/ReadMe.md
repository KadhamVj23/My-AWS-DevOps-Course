# AWS Basics for DevOps

## IAM - Identity And Access Management

IAM defines who does what in AWS. Basically it will make your work easier, when you have to give access to certain group of people like such as what the finance team can do in AWS, or the developers team can do in AWS, and apart form those tasks they will not be able to do other things.

So, in short it allows you to manage identites and permissions and it is a free service. And everything you do is gated thorugh IAM.

Lets see a few **building blocks** of IAM:

1. IAM Users

2. IAM Groups

3. IAM Policies

4. IAM Roles


### IAM Users:

If you want to give access to persons in your company to the AWS console, you will need to create the user in the console and that user is called IAM user. You might have testers, developers, finance team members, and for each user you need to create a username and a password. This is giverned by IAM users.

- IAM user has a username and password and they have access to console(console means dashboard of AWS)

- They can have access keys. These are the secret keys by using which developers can access AWS resources using command line.

### IAM Groups:

It is a collection of users with shared permissions. 

Lets say you have many devs in your org and you want to give some perimissions to them. So, giving them the permission individually will take time and it is not best practise also. So what you do is you create a group that group is called **IAM Groups** and then you assign a policy to the group and then you can add as many users you want, instead of giving them seperately.

Example:
Group: Developers -> Policy: PowerUserAccess
Group: Viewers -> Policy: ReadOnlyAccess.


### IAM Roles:

Lets say you have a service AWS Lambda, and it needs to interact with S3 bucket for some processing or work, but it is not possible for it to access S3 bucket, in that case you can create a temporary role and give permission to AWS Lambda so that it will interact with S3 bucket and then after the work is finished it will come back to its orginal state without the role.

It is a temporary access assumed by users, apps or services. 

- It doesn't require permenant access.
- Best practise for Lambda, EC2, EKS and CI/CD.


### IAM Policies:

IAM Policies are nothing but **Permissions** that are defined by you and can be used by Users, Roles and Groups.

- Policies are defined using JSON documents, so it is JSON like syntax.