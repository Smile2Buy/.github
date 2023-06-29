# Development log
> [Details](https://github.com/orgs/Smile2Buy/projects/1)

## Implementation history
- [x] ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Init repo by adding some GitHub Actions; Drafter, Labeler
- [x] ![Infra badge](https://img.shields.io/badge/infra-7B42BC) Bootstrap basic AWS architecture; VPC, Subnets, Internet Gateway, NAT Gateway, Elastic IP, Route tables. Verified as follows,
  - [x] VPC Creation: The specified VPC is created with the correct CIDR block.
  - [x] Subnet Creation: Subnets (private, public) are created within the VPC with correct CIDR blocks.
  - [x] Route Table Association: Each subnet have the correct route table associated with it.
    - [x] Public subnet that route through an Internet Gateway. (w. internet access)
    - [x] Private subnet that routes through a NAT gateway. (w.o. internet access)
  - [ ] Access Control: Ensure that the correct security groups, Network ACLs, and other access control mechanisms are in place and only allow traffic that you expect
