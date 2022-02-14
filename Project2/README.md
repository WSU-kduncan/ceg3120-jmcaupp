# Part One:

### VPC
![VPC](https://github.com/WSU-kduncan/ceg3120-jmcaupp/blob/main/Project2/images/VPC.png)
10.0.0.0/24 IP range is specified

### Subnet
![subnet](https://github.com/WSU-kduncan/ceg3120-jmcaupp/blob/main/Project2/images/Subnet.png)
10.0.0.0/28 subnet
attached to the proper VPC

### Internet Gateway
![gateway](https://github.com/WSU-kduncan/ceg3120-jmcaupp/blob/main/Project2/images/Gateway.png)
attached to the proper VPC

### Route Table
![routetable](https://github.com/WSU-kduncan/ceg3120-jmcaupp/blob/main/Project2/images/RouteTable.png)
attached to the proper VPC
associated with the proper subnet
all outward traffic directed to the created gateway

### Security Group
![securitygroup](https://github.com/WSU-kduncan/ceg3120-jmcaupp/blob/main/Project2/images/SecurityGroup.png)
inbound rules:
![inbound](https://github.com/WSU-kduncan/ceg3120-jmcaupp/blob/main/Project2/images/InboundRules.png)

# Part Two:

### Choose AMI / Choose Instance Type
I created an instance of Amazon Linux 2, which has a default user name of ec2-user.
After selecting this AMI, I made sure to choose the instance with the Free tier eligible.

### Configure Instance
In step 3, I made sure to attach this instance to the VPC I just created by choosing it in the dropdown menu. I also disabled the option to auto assign a public IP. This will prevent me from having to reconfigure and "fix" my settings later should Amazon choose to reassign this IP. Instead, I will assign an elastic IP at a future step.

### Add Storage
The default size in this step was set to 8, I increased it to 16 just to have plenty of space.

### Add Tags
Key: Name 
Value: CAUPP-EC2

### Configure Security Group
Click select an existing security group and choose the security group created in the last step

### Review and Launch
The final step after clicking Launch is to ensure you have key pairs set up to use for this instance. The default selection is to use an existing key pair which works just fine for our purposes.

### Elastic IP
Now is the time to generate and associate an Elastic IP address. Under Network & Security, select Elastic IPs. Click Allocate Elastic IP Address, don't forget to give it a name tag, and click Allocate again. Once it is allocated, select it click the dropdown Actions menu and associate it to your newly created instance.

![instance](https://github.com/WSU-kduncan/ceg3120-jmcaupp/blob/main/Project2/images/Instance.png)
