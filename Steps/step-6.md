## Strore Credentials in Jenkins

### Storing Dockerhub Credentials

- Open Jenkins in a browser.
- Click on Credentials.
- Click on System.
- Click on Global credentials.
- Click on Add Credentials.
- Select Username with password.
- Enter the username and password of your Dockerhub account.
- Click on OK.

![net-34](https://github.com/mathesh-me/ci-cd-dotnet-app-deployment/assets/144098846/b96f2a47-95fe-4b44-9a34-1b898b9bbad3)


### Storing SonarQube Credentials

#### How to get SonarQube Credentials

- Open SonarQube in a browser.
- Click on Administration.
- Click on Security.
- Click on Users.

![net-18](https://github.com/mathesh-me/ci-cd-dotnet-app-deployment/assets/144098846/e2c68c00-20a2-440a-9953-96206b8d1111)

![net-19](https://github.com/mathesh-me/ci-cd-dotnet-app-deployment/assets/144098846/8c0ad9b2-8b74-42d9-9b33-2cb50d49e388)


#### How to store SonarQube Credentials in Jenkins

- Open Jenkins in a browser.
- Click on Credentials.
- Click on System.
- Click on Global credentials.
- Click on Add Credentials.
- Select Secret text.
- Enter the generated token in the Secret field.
- Enter the ID as `sonar-token`.
- Enter the description as `sonar-token`.
- Click on OK.

![net-20](https://github.com/mathesh-me/ci-cd-dotnet-app-deployment/assets/144098846/1cd08790-4ac6-413e-b188-8f35f16c6a00)
