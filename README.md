Follow these steps in Jenkins - 
1. Create a new project in Jenkins.
2. Add the GitHub URL of this project in the Source Code Management section.
3. Select 'GitHub hook trigger for GITScm polling' in 'Build Triggers' section.
4. Add the build steps to start the container and save the project.

Follow these steps in this GitHub Project:
1. Go to the settings of this project and in the Webhooks section, Click on 'Add webhook'.
2. In the payload URL, add the public IP address with the port on which you are accessing Jenkins and 'github-webhook/'.
3. So, it will look like 'http://18.119.116.148:8080/github-webhook/'.
4. Select 'application/json' in Content Type and select 'Just the push event' in next option and click on 'Add webhook'.
5. Now, make any changes in this project and commit them.

In Jenkins, check that one build will be created after you commit.
So, GitHub webhooks are used to trigger a build in Jenkins whenever someone commits to the project if we select 'Just the push event'.
