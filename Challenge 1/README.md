Challenge #1

A 3-tier environment is a common setup. Use a tool of your choosing/familiarity create these resources. Please remember we will not be judged on the outcome but more focusing on the approach, style and reproducibility.
 
Link Referred - https://github.com/Azure/azure-quickstart-templates/tree/master/application-workloads/redhat/rhel-3tier-iaas


This template will deploy:

1. One Virtual Network with four subnets
2. 4 Network Security Group, one for each subnet
3. External Load Balancer to load balance Web Traffic(HTTP & HTTPS) to web servers
4. Internal Load Balancer to load balance traffic for app VM's
5. 2 Public IP’s, one for external Load balancer and other for Jump VM
6. Virtual Machine Availability sets for Web Tier, Application Tier and Database tier
7. One Jump VM to faclitate RDP access to all other tier VMs
8. Multiple windows VMs with nics
