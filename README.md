# Path Based Webapp
Geo Redundant Path Based Routing

# Motivation:
We may have built an application but never thought about distributing it at scale, let alone globally. So, in this post, I will be showing you how we can leverage Azure Services like Azure Traffic Manager, Azure Load Balancer, Application gateway, and Azure Front Door to scale our distribution to people around the globe.

# Architecture:
![architecture](https://user-images.githubusercontent.com/13358738/123514207-7414ae80-d6b1-11eb-9592-7ef0f838b5c8.png)

# Prerequisites:
1. Azure Virtual Machine
2. Azure Virtual Machine Scale Sets
3. Azure Load Balancer
4. Azure Traffic Manager
5. Azure Application Gateway
6. Azure Front Door

# Replication Steps:
As the VMSS template couldn't be exporeted, there is no ARM template for it. I have written all the replication steps on my blog post

# Useful Commands:

- Command for VM
```bash
#!/bin/bash
sudo apt update -y
sudo apt install apache2 -y
```

- Command for VMSS
```bash
#!/bin/bash
sudo apt update -y
sudo apt install apache2 -y
echo "<html><h2>This is images farmed page</h2></html>" > images.html
sudo cp images.html /var/www/html/
```
