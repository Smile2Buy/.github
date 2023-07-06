# Development log
> [Check here for details!](https://github.com/orgs/Smile2Buy/projects/1)

## Infra implementation history
### Nested Implementation
- ![Infra badge](https://img.shields.io/badge/infra-7B42BC) VPC
- ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Subnets
  - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Public Subnet
    - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Set 1 AZ
    - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Internet Gateway
    - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Route-table & Route-table-association
  - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Private Subnet with 
    - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Set 1 AZ
    - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) NAT Gateway & Elastic IP
    - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Route-table & Route-table-association
### Flat Implementation
- ![Infra badge](https://img.shields.io/badge/infra-7B42BC) VPC
- ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Subnets
  - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Public Subnet
    - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Set 2 AZs
    - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Internet Gateway
    - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Route-table & Route-table-association
  - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Private Subnet -1az
    - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Set 2 AZs
    - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) NAT Gateway & Elastic IP
    - ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Route-table & Route-table-association
### GitOps
- ![Infra badge](https://img.shields.io/badge/infra-7B42BC) AutoLabel -- Attach labels of type and domain to the opened PR
- ![Infra badge](https://img.shields.io/badge/infra-7B42BC) ReleaseDrafter -- Build a drafter of release note when code push to [main] branch occurs
- ![Infra badge](https://img.shields.io/badge/infra-7B42BC) HistorySpoke -- Send message to Hisory-hub repository when README.md has been changed
### CDK Implementation
