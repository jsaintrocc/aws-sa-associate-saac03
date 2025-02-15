* 0100 - 0500 Unsorted
    * IAM is a globally resilient service. So any data is always secure across all AWS Regions
    * Connecting to EC2 uses port 3389 for Windows instances (The remote desktop protocol)
    * Connecting to EC2 uses port 22 on Linux instances (The ssh protocol)
    * IAM Policy statement priority: 1: Explicit DENY, 2: Explicit ALLOW, 3: default DENY (Implicit) (DENY/ALLOW/DENY)
    * If you can picture one thing, a named thing 99% of the time you want an IAM User
    * Authencation: Prove who you are
    * Autorization: Check what you can do
    * 5000 IAM users per account
    * You cannot login to an IAM Group
    * There isn't a built in ALL USERS group in IAM by default
    * IAM Groups are not a true identity. They can't be referenced as a principal in a policy
* 0500-iam_accounts_and_aws_orgs
    * External accounts/identities can't be used in AWS directly
    * For mobile applications using IAM Roles and IAM federation is the preferred method
    * Master account, management account, payer account are mean the same thing for an organization. Account used to create an org and used to pay the bill for an org
    * For organizations the architectural pattern is a single account for identities and then roles for each identity to access the other accounts under an org.

