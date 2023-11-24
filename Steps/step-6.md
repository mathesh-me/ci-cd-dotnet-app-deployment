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

// Image will be added here

### Storing SonarQube Credentials

#### How to get SonarQube Credentials

- Open SonarQube in a browser.
- Click on Administration.
- Click on Security.
- Click on Users.

// Image will be added here

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

// Image will be added here