# Cloudformation-Udagram

#### URL for a working example. 
http://serve-webap-12srdabswiwqi-1913077059.us-west-2.elb.amazonaws.com/

This project describes the process of provisioning an AWS cloud infrastructure using cloudformation. 
We will be deploying a simple web application hosted on EC2 instances that are deployed on private subnets which in turn are being access through a load balancer in the public subnet. As mentioned, the whole infrastructure is automated using cloudformation templates. 

![GitHub Logo](/cloudformation-infrastructure.png)

## How to run this example.
Note that, this project assumes a s3 bucket is available to be queried from. 
### Clone this git repository locally.
````
git clone https://github.com/vSivarajah/Cloudformation-Udagram.git

cd Cloudformation-Udagram
````


### Provision the network layer. 
````
./create.sh network-infrastructure network/network-infrastructure.yml network/network-infrastructure.json
````

### Provision the server layer
`````
./create.sh server-infrastructure servers/server-infrastructure.yaml servers/server-infrastructure.json
`````



