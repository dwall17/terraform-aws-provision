# terraform-aws-provision

## Terraform project in which the following AWS resources are created:
1. VPC
2. Internet Gateway (so traffic can be sent to the Internet)
3. Custom Route Table (this is needed for the subnet)
4. Subnet (anytime you create a subent you have to assign it to a route table or they'll get assigned to the VPC's default route table
5. Associate subnet with route table
6. Security Group (responsible for determining what kind of traffic reaches the EC2 instance and outgoing traffic)
7. Custom network interface with an IP in the subnet that was created in step 4
8. Elastic IP, then assign it to the network interface
9. Ubuntu server && install/enable apache2
