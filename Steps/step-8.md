## Configuring Webhook

### Follow the below steps to configure webhook in GitHub Repository(Where application code is stored) so that whenever a developer pushes code to GitHub, it will automatically trigger the Jenkins job.
- We are going to configure webhook in GitHub Repository(Where application code is stored) so that whenever a developer pushes code to GitHub, it will automatically trigger the Jenkins job.
- Open Jenkins in a browser.
- Click on the pipeline job.
- Click on Configure.
- Scroll down to Build Triggers.
- Select GitHub hook trigger for GITScm polling.
- Click on Save.
- Open GitHub in a browser.
- Click on the repository.
- Click on Settings.
- Click on Webhooks.
- Click on Add webhook.
- Enter the Payload URL as `http://<Jenkins-IP>:8080/github-webhook/`.
- Enter the Content type as `application/json`.
- Enter the Secret as `Jenkins`.
- Select Let me select individual events.
- Select Pushes.
- Click on Add webhook.
