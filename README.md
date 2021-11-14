# Network design

This network diagram consists out of 3 subnets.

Yellow Private Subnet: On the top left in the yellow circle, there is a private subnet that supports up to 30 hosts. Router R1 in this subnet is directly connected to Router R2 in the Blue private subnet. R1 is also directly connected to R3 in the red subnet, R1 has no direct connectivity to the public internet. It has to go through R2 and R5 (NAT gateway) before it reaches the Internet Gateway R4, or it has to go through R3 and then to R4.

Blue Private Subnet with NAT Gateway: The blue subnet supports 62 hosts and contains R2 and R5 (NAT gateway). R5 is directly connected to R4 in the Red Public subnet, the NAT gateway has a direct link to the internet through the Internet Gateway R4.

Red Public Subnet with Internet Gateway: The red subnet supports up to 14 hosts and contains R3 and R4 (Internet Gateway). R4 is directly connected to R3 and provides Internet connectivity to R3. R3 is also directly connected to R1 in the yellow subnet.
