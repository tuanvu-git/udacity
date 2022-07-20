### Project Title - Deploy a high-availability web app using CloudFormation
This folder provides the starter code for the "ND9991 - C2- Infrastructure as Code - Deploy a high-availability web app using CloudFormation" project. This folder contains the following files:


#### final-project-starter.yml
Students have to write the CloudFormation code using this YAML template for building the cloud infrastructure, as required for the project. 

#### server-parameters.json
Students may use a JSON file for increasing the generic nature of the YAML code. For example, the JSON file contains a "ParameterKey" as "EnvironmentName" and "ParameterValue" as "UdacityProject". 

In YAML code, the `${EnvironmentName}` would be substituted with `UdacityProject` accordingly.

###  STUDENT NOTE
1.  because using S3 inside EC2 instance is optional so I skipped this step and don't need to create IAM
2.  In Project Requirements "server specs" have scenario
"You'll need two vCPUs and at least 4GB of RAM. The Operating System to be used is Ubuntu 18. So, choose an Instance size and Machine Image (AMI) that best fits this spec."
but for low charging, I set up EC2 instance type and instance Number don't meed requirement
3.  I used my docker image to run in EC2 (see UserData in LaunchConfiguration) instead of copying file HTML into EC2
4.  DNS_NAME of load balancer: ...