## Deploying Application

- Go to the Jenkins Dashboard and click on the pipeline job.
- Click on **Build Now**.
![net-30](https://github.com/mathesh-me/ci-cd-dotnet-app-deployment/assets/144098846/ff4f7eee-8215-4e00-ae7a-6c05e7dc99ec)
![net-31](https://github.com/mathesh-me/ci-cd-dotnet-app-deployment/assets/144098846/584cc1d0-e34-473b-a5d7-f42c08118727)

- The build will start and you can see the progress in the console output.
- Once the build is completed, you can see the application running on the public IP of the EC2 instance.
- You can also see the application running on the public IP of the EC2 instance.
- You can see the .NET in the browser. By default, the application runs on port 5000.
- So, you have to open the port 5000 in the security group of the EC2 instance.
![net-37](https://github.com/mathesh-me/ci-cd-dotnet-app-deployment/assets/144098846/8519775f-fd52-4537-8bb6-468d9df2c8e0)

- Now, you can access the application using the URL `http://<public-ip>:5000`.
![net-38](https://github.com/mathesh-me/ci-cd-dotnet-app-deployment/assets/144098846/f9d36c37-229b-44bd-83d6-5581eebca057)
