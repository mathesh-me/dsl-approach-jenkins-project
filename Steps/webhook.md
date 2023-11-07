## Steps for configuring webhook for the pipeline

- As we already given in the Jenkins job configuration to trigger the Maven job when there is any changes in the GitHub repository, we need to configure the webhook in the GitHub repository.(As per DSl script)
- But We need to configure for Seed job Manually. For that we need to go to jenkins and configure the webhook for the seed job.
    1. Go to the Jenkins server
    2. Click on the Seed job in the dashboard
    3. Click on 'Configure' in the left side of the dashboard
    4. Scroll down to the 'Build Triggers' section
    5. Select 'GitHub hook trigger for GITScm polling'
    6. Click 'Save'
- Now , Repeat the below steps for the two repositories(The repositories which contains code for both jobs if you kept the code for both jobs in same repository if need to do that on that particular repository) which you have created in the GitHub.
- Go to the GitHub repository
- Click on 'Settings' in the right side of the repository
- Click on 'Webhooks' in the left side of the repository
- Click on 'Add webhook'
- Give the Payload URL as
```
http://<Jenkins-IP>:8080/github-webhook/
```
- Give the Content type as 'application/json'
- Give the Secret as 'mysecret'
- Select 'Just the push event' in the 'Which events would you like to trigger this webhook?' section
- Click 'Add webhook'
- Now if you make any changes in the GitHub repository the pipeline will automatically start building the project.