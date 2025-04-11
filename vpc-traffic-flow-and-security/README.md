## VPC Traffic Flow and Security

**Step 1**: Create a VPC, subnet, and configure the IGW. 

**Step 2**: Create a Route Table
- Select the routes tab and edit routes 
- Add a route 
    - Choose the 0.0.0.0/0 (this is used to send everything else to the internet when no other specific route is found.) 
    - Target: Choose IGW (Internet Gateway) you’ve created earlier 
    - Save
- Click subnet association tab 
    - Click edit subnet association 
    - Click the subnet you’ve created

**Step 3**: Create a security group 
Note: Security groups are responsible for the security of the resources. They can set rules who can enter or leave the resources based on their IP addresses, protocols, and port numbers. 
- Under the left navigation tab, find the security section and click the security groups.  
- Click Create Security group and add all the necessary information. 
- Add inbound rule (click HTTP and for the source, click anywhere in IPv4)

**Step 4**: Create a NACL (Network Access List)
Note: NACL controls traffic for the whole subnet level. 
    - Add all the necessary information
    - Choose your VPC 
    - Click Create 
- Edit Inbound Rules
    - Add new rule 
    - Type Rule 100
    - All Traffic 
    - Save
- Edit Outbound Rules
    - Add new rule
    - Type Rule 100
    - All traffic
    - Save

**Step 5**: Click subnet Association tab
- Select your subnet
- Save
