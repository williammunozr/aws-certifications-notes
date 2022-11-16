# AWS Accounts

- An AWS Account is a container for `identities` (users) and `resources`.
- When creating an AWS Account you provide an account name e.g. PROD, a `unique email address` and a `credit card`.
- Every account has an `Account Root User`. 
- The `Account Root User`has full control over all of this `AWS Account` and any `resources` created within it & cannot be restricted.
- Account payment method.
- `Resources` bill to the `AWS Account` payment method as they are consumed.
- Identity and Access Management (`IAM`) Users, Groups and Roles can also be created and given FULL Or LIMITED permissions.
- `AWS Accounts` can contain the impact of admin errors, or exploits by bad actors. Use separate accounts for separate things (DEV, TEST, PROD), teams, products or clients.
- By default all access to an `AWS Account` & resources is denied except for the `Account Root User`.
- External identities can be granted access.

## Resources

- [AWS Accounts - AWS SA Associate](https://learn.cantrill.io/courses/1820301/lectures/41301458)
- [AWS Accounts](https://aws.amazon.com/account/)
- [AWS Organizations terminology and concepts](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_getting-started_concepts.html)