𝐕𝐏𝐂 𝐰𝐢𝐭𝐡 𝐏𝐮𝐛𝐥𝐢𝐜 𝐏𝐫𝐢𝐯𝐚𝐭𝐞 𝐒𝐮𝐛𝐧𝐞𝐭 𝐢𝐧 𝐏𝐫𝐨𝐝𝐮𝐜𝐭𝐢𝐨𝐧


𝐀𝐛𝐨𝐮𝐭 𝐭𝐡𝐞 𝐏𝐫𝐨𝐣𝐞𝐜𝐭


This example demonstrates how to create a VPC that you can use for servers in a production environment.
To improve resiliency, you deploy the servers in two Availability Zones, by using an Auto Scaling group and an Application Load Balancer. For additional security, you deploy the servers in private subnets. The servers receive requests through the load balancer. The servers can connect to the internet by using a NAT gateway. To improve resiliency, you deploy the NAT gateway in both Availability Zones.

𝐎𝐯𝐞𝐫𝐯𝐢𝐞𝐰

The VPC has public subnets and private subnets in two Availability Zones.
Each public subnet contains a NAT gateway and a load balancer node.
The servers run in the private subnets, are launched and terminated by using an Auto Scaling group, and receive traffic from the load balancer.
The servers can connect to the internet by using the NAT gateway.
