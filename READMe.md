# Let's create a Continuous Integration and Continuous Delivery/Deployment (CICD) pipeline
## Jenkins
### Webhooks with Git-hub
#### Automated Testing using Jenkins
#### Deployment on AWS EC2

- Jenkins Workflow
  
![](images/jenkins.png)

  ##### Contiounus Integration Continuous Delivery/Deployment 
![](images/CICD.png)

###### Let's break it down 
  ![](images/cicd_jenkins.png)

### For deployment job in Jenkins
- In the execute shell of CD job

```
# we need to by pass the key asking stage with below command:
ssh -A -o "StrictHostKeyChecking=no" ubuntu@ec2-ip << EOF	

# create an env to connect to db
# navigate to app folder
# kill any existing pm2 process just in case
# launch the app
    

EOF
```