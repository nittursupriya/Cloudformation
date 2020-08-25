# Cloudformation
Creating Infrastructure as a Code template to deploy resources using cloud formation on AWS
Activity Template YAML File contains the following code steps:
Region: Ireland
Part1:
 1. Define a VPC
 2. Add a subnet to your VPC which maps public IP addresses to the EC2 instances launched inside it.
 3. Add a route table to your VPC and associate it with your Subnet.
 4. Define an IG and attach to your VPC.
 5. Add a route in your route table for the Internet Access(CIDR IP: 0.0.0.0/0) via your Internet Gateway.
 6. Define an EC2 instance in your public subnet.
 7. Create a stack from the template.
 
 Part 2:
  1. Edit your template and add a security group resource which has an ingress rule allowing ping requests (ICMP protocol)
  2. Attach the security group to EC2 Instance.
  3. Update the stack with the latest template.
  4. Test whether your EC2 instance is reachable by pinging to the public IP address.
