Naveen automated ci-cd pipeline project
This project shows how to use Jenkins to automatically build, test, and package a web application whenever code is pushed to GitHub.
It helps developers check that the latest code is always working and ready to deploy.

What This Project Does
Connects Jenkins with a GitHub repository
Automatically pulls new code when changes are made
Installs dependencies using npm
Runs tests using Jest
Builds the project and saves the build files (artifacts)
Shows the build result (success or failure)

Tools Used
Tool	Purpose
Jenkins	Continuous Integration (CI) tool
GitHub	Source code hosting
Node.js + npm	Web app and dependency manager
Jest	Testing framework
Git	Version control system

Pipeline Stages
Checkout Code – Jenkins pulls code from GitHub
Install Dependencies – Runs npm install
Run Tests – Runs npm test (using Jest)
Build Package – Runs npm run build
Archive Artifacts – Saves build output in Jenkins

Step 1: Install Required Tools
Install Jenkins, Node.js, npm, and Git.
Step 2: Configure Jenkins
Open Jenkins → http://localhost:8080
Install Suggested Plugins
Add GitHub credentials (username + personal access token)
Step 3: Create a Jenkins Pipeline
Click New Item → Pipeline
Choose Pipeline script from SCM
Add your GitHub repo link
Set Script Path to Jenkinsfile
Save and click Build Now

Output
Jenkins automatically builds your project when you push new code
Shows all stages (Checkout, Install, Test, Build, Archive)
Saves final build artifacts
Displays success/failure in the dashboard
