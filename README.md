### Project Title - Deploy a high-availability web app using CloudFormation

This project have two seperate files

1. Network Configuration
2. Server Configuration

To setup the project kindly run the following command

1. Setup network: "aws cloudformation create-stack --stack-name project1-network --region us-east-1 --template-body file://network.yml --parameters file://network-parameters.json"

2. Setup server: "aws cloudformation create-stack --stack-name project1-servers --region us-east-1 --template-body file://servers.yml --parameters file://server-parameters.json"

From the server stack (project1-servers) outputs you can get the Load balancer url (key: LoadBalancerUrl)

3. Url of working site: http://proje-WebAp-1R0JH9M361OVE-1634126924.us-east-1.elb.amazonaws.com