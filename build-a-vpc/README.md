## Steps in Building a VPC
**Step 1**: Create a VPC 
- Choose VPC only and configure the necessary information 
- After creating a VPC, create a subnet. (Where you can organize your resources with a similar rules and restrictions) Subnets can be private and public. 
- Choose the first AZ, configure the IPv4 VPC CIDR block and the IPv4 subnet CIDR block.

**Step 2**: Edit subnet settings
- Enable auto assign public IPv4 address
    - When you click this option, you don’t need to manually create a public IP address. 

**Step 3**: Create an IGW
- Attach it to the public subnet we created earlier.
