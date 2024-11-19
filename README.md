# AWS-CI-PROJECT

## Set Up GitHub Repository ##
The first step in our CI journey is to set up a GitHub repository to store our Python application's source code. If you already have a repository, feel free to skip this step. Otherwise, let's create a new repository on GitHub by following these steps: <br> 

Go to github.com and sign in to your account.<br>
1. Click on the "+" button in the top-right corner and select "New repository."
2.Give your repository a name and an optional description.
3. Choose the appropriate visibility option based on your needs.
4. Initialize the repository with a README file.
4. Click on the "Create repository" button to create your new GitHub repository.
<br>Great! Now that we have our repository set up, we can move on to the next step.

## Create an AWS CodePipeline
In this step, we'll create an AWS CodePipeline to automate the continuous integration process for our Python (flask) application. AWS CodePipeline will orchestrate the flow of changes from our GitHub repository to the deployment of our application. Let's set it up:

1. Go to the AWS Management Console and navigate to the AWS CodePipeline service.
2. Click on the "Create pipeline" button.
3. Provide a name for your pipeline and click on the "Next" button.
4. For the source stage, select "GitHub" as the source provider.
5. Connect your GitHub account to AWS CodePipeline and select your repository.
6. Choose the branch you want to use for your pipeline.
7. In the build stage, select "AWS CodeBuild" as the build provider.
8. Create a new CodeBuild project by clicking on the "Create project" button.
9. Configure the CodeBuild project with the necessary settings for your Python application, such as the build environment, build commands, and artifacts.
10. Save the CodeBuild project and go back to CodePipeline.
11. Continue configuring the pipeline stages, such as deploying your application using AWS Elastic Beanstalk or any other suitable deployment option.
12. Review the pipeline configuration and click on the "Create pipeline" button to create your AWS CodePipeline.
    
Awesome job! We now have our pipeline ready to roll. Let's move on to the next step to set up AWS CodeBuild.
