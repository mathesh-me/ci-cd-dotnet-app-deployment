## Install and Configure Jenkins

- SSH into the EC2 instance created in [Step-1](./Steps/step-1.md).
```
ssh -i <path-to-pem-file> ubuntu@<ec2-instance-public-ip>
```
- Install Jenkins.
```
sudo apt-get update

curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee \
    /usr/share/keyrings/jenkins-keyring.asc > /dev/null
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
    https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
    /etc/apt/sources.list.d/jenkins.list > /dev/null

sudo apt-get update
sudo apt-get install fontconfig openjdk-11-jre
sudo apt-get install jenkins

sudo systemctl enable jenkins
sudo systemctl start jenkins
sudo systemctl status jenkins
```
- Now Jenkins is installed and running on port 8080. To access Jenkins, open the following URL in a browser.
```
http://<ec2-instance-public-ip>:8080
```
- To get the initial admin password, run the following command.
```
sudo cat /var/lib/jenkins/secrets/initialAdminPassword
```
// Image will be added here

- Install the suggested plugins.
// Image will be added here

- Create an admin user.
// Image will be added here

- Jenkins is now ready to use.
// Image will be added here




