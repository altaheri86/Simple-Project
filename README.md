# Create Jenkins | Run Jenkins Pipeline using Jenkinsfile

## Step 1:
### Install Jenkins and other dependencies
```bash
# Create sh file with the commands as shown in the install.sh file 
vim install.sh
chmod +x install.sh 
./install.sh
```
## Step 2:
### Setup Jenkins
```bash
# Access Jenkins using the EC2 IPv4-Public-DNS:8080
```
---

## Step 3:
### Add Github and Dockerhub credentials in Jenkins
`Manage Jenkins > Manage Credentials > Global > Add Credentials`

Make sure to use Dockerhub access token instaed of the password
`Dockerhub > Account Settings > Security > New Access Token`

---
## Step 4: 
### Create Jenkins Pipeline 
`Choose pipeline, if not found you can install it from Manage Jenkins > Manage Plugins`

In **Pipeline Section** in the end of the page choose **Pipeline script from SCM** > Add **Gihub Repository link** > Using **Github Credentials**

`Make usre you choose the right branch and the right path of the Jenkinsfile`

---

