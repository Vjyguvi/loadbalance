# Task
> 1. Create a S3 bucket, with no public access and upload files to the bucket
>
### ( Block Public Access Settings )
![Screenshot block public](https://github.com/Vjyguvi/loadbalance/assets/150816386/67acc356-a1e6-475a-8040-c1cd6b9e1229)

### ( Public access denied )

>> I uploaded a file and attempted to access it publicly . Access denied.

![Screenshot public access denied](https://github.com/Vjyguvi/loadbalance/assets/150816386/b56a1677-541d-4578-95c2-daf2d283d773)

> 2. Launch two ec2-instances and connect it to a application load balancer, where the output traffic from the server must be an load balancer IP address
###### Two EC2 instances were created with NGINX installed. On one server, the paths are /var/www/html/main and /var/www/html/user.
######  Subsequently, two target groups were created for the two servers separately.
###### Following that, a load balancer was created, and rules were added with path conditions mapped to the respective target groups.
###### Finally, I tried to access the servers through the load balancer DNS with different paths, and I was able to access the two different servers using the Application Load Balancer.

### ( Create Target Group )

![Screenshot Target group](https://github.com/Vjyguvi/loadbalance/assets/150816386/c50c4dc9-e92d-45d6-b9b8-af0b91e96307)

### ( Add Rules in Loadbalancer )

![Screenshot rules load balancer](https://github.com/Vjyguvi/loadbalance/assets/150816386/b202dfc1-896c-4283-a8cd-de171a163553)

### ( Output using loadbalancer DNS with path /main )

![Screenshot dns main path](https://github.com/Vjyguvi/loadbalance/assets/150816386/1a0d515c-6323-427e-8fb2-2e9d0c636036)

### ( Output using loadbalancer DNS with path /user )

![Screenshot DNS user path](https://github.com/Vjyguvi/loadbalance/assets/150816386/204ea3ec-6a64-4cdc-bf9a-806e05f96737)
