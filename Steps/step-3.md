## Install tools on Virtual machine

### Step 1:
- SSH into the EC2 instance created in [Step-1](./Steps/step-1.md).
```
ssh -i <path-to-pem-file> ubuntu@<ec2-instance-public-ip>
```

- Install Docker.
```
sudo apt-get update
sudo apt-get install docker.io -y
sudo usermod -aG docker $USER
sudo usermod -aG docker Jenkins
sudo chmod 777 /var/run/docker.sock
sudo chown jenkins:docker /var/run/docker.sock
sudo docker ps
```

### Step 2:
- After installing Docker, Spin-up a `sonar` container using the following command.
```
docker run -d --name sonar -p 9000:9000 sonarqube:lts-community
```

- Now, SonarQube is running on port 9000. To access SonarQube, open the port 9000 in the security group of the EC2 instance and open the following URL in a browser.
```
http://<ec2-instance-public-ip>:9000
```

- Login to SonarQube using the default credentials.
```
Username: admin
Password: admin
```

// Image will be added here
// Image will be added here
// Image will be added here

### Step 3:
- Install Trivy.
```
sudo apt-get install wget apt-transport-https gnupg lsb-release

wget -qO - https://aquasecurity.github.io/trivy-repo/deb/public.key | gpg --dearmor | sudo tee /usr/share/keyrings/trivy.gpg > /dev/null

echo "deb [signed-by=/usr/share/keyrings/trivy.gpg] https://aquasecurity.github.io/trivy-repo/deb $(lsb_release -sc) main" | sudo tee -a /etc/apt/sources.list.d/trivy.list

sudo apt-get update

sudo apt-get install trivy -y
```

### Step 4:
- Install make.
```
sudo apt-get install make -y
```


