# COMP2156_Group19_Assignment

1. Project Title 
2. Group Members: 
o List each member with their Student ID and GitHub 
username. 
3. Project Description: 
o Brief overview of what the assignment entails. 
4. Instructions: 
o How to set up the project locally. 
5. CI/CD Details: 
o Information about the CI pipeline setup. 
6. Branching Strategy: 
o Explain the branching conventions used. 



Just so there's something in the read me, here are the assignment instructions

Group Assignment 
COMP 2156 – DevOps For System Administration
 Total: 16% (100 Points) 
Submission Deadline: Saturday, 15th Feb 2025, 11:59 pm (Week06) 
Completing a group assignment involving GitHub collaboration, branching, 
and continuous integration (CI) can be streamlined by following a structured 
approach. Below is a step-by-step guide to help your group successfully 
complete the COMP 2156 - DevOps For System Administration 
assignment: 
1. Forming Your Group 
• Group Size: Ensure your group has 3 to 4 members. 
• Communication: Decide on a primary communication channel (e.g., 
Slack, email) to coordinate tasks and share updates. 
2. Creating the GitHub Repository 
• Repository Name Format: COMP2156_Group#_Assignment (e.g., 
COMP2156_Group1_Assignment). 
• Repository Type: Public 
• Repository Owner: Only one member (Leader) will create the 
repository. 
Reference Steps: 
1. Leader Creates Repository: 
o Log in to GitHub. 
o Click on "New" to create a new repository. 
o Enter the repository name following the specified format. 
o Set the repository to Public. 
o Initialize with a README.md if desired. 
2. Add Collaborators: 
o Go to the repository’s Settings. 
o Navigate to "Manage access". 
o Click "Invite a collaborator" and add the GitHub usernames 
of the other group members. 
o Assign appropriate permissions (e.g., Write access). 
3. Assigning Roles 
The leader will add the remaining group members as collaborators with the 
necessary permissions to push and manage branches. 
• Leader/Owner: Manages the repository and adds collaborators. 
• Collaborators: Clone the repository and contribute via their branches. 
4.  Branch Management 
Each member will create a branch named with their STUDENTID-Name 
• Branch Naming Convention: STUDENTID-Name (e.g., 1023756-Pritesh). 
Reference Steps for Each Member: 
1. Clone the Repository: 
git clone https://github.com/YourUsername/COMP2156_Group#_Assignment.git 
2. Navigate to the Repository: 
cd COMP2156_Group#_Assignment 
3. Create and Switch to Your Branch: 
git checkout -b STUDENTID-Name 
4. Push the Branch to GitHub: 
git push -u origin STUDENTID-Name 
5. Setting Up Continuous Integration (CI) 
One member will integrate the repository with GitHub Actions or another 
CI tool to automate the build and testing processes. 
• CI Tools: GitHub Actions (recommended) or any free CI tool of your 
choice. 
• Responsibility: Only the Leader sets up the CI pipeline. 
Using GitHub Actions: 
1. Navigate to the Repository on GitHub. 
2. Go to the "Actions" Tab. 
3. Set Up a Workflow: 
o Choose a template or create a new workflow. 
o For example, a basic workflow can be set to run on push 
events. 
4. Commit the Workflow File: 
o This file will be located in .github/workflows/. 
Sample GitHub Actions Workflow (ci.yml): Modify the workflow 
according to your project’s requirements. 
name: GitHub Actions Demo 
run-name: ${{ github.actor }} is testing out GitHub Actions 
on: [push] 
�
�
 jobs: 
Explore-GitHub-Actions: 
runs-on: ubuntu-latest 
steps: - run: echo "
 🎉
 🐧
 The job was automatically triggered by a ${{ github.event_name }} event." - run: echo "
 🔎
 This job is now running on a ${{ runner.os }} server hosted by GitHub!" - run: echo "
 The name of your branch is ${{ github.ref }} and your repository is ${{ 
github.repository }}." - name: Check out repository code 
uses: actions/checkout@v4 - run: echo "
 💡
 🖥
 The ${{ github.repository }} repository has been cloned to the runner." - run: echo "
 🍏
 The workflow is now ready to test your code on the runner." - name: List files in the repository 
run: | 
ls ${{ github.workspace }} - run: echo "
 This job's status is ${{ job.status }}." 
6. Making Commits and Creating Files 
Each Member Must: 
• Create at Least 10 Commits: 
o Regularly commit changes with meaningful messages. 
• Create 3 Specific Files: (Think of your own content) 
o Format: Studentid_filename.txt (e.g., 1023756_gb.txt) 
o Contents: 
1. Studentid_gb.txt: Information about George Brown College. 
2. Studentid_devops.txt: Information about the COMP 3104 
DevOps course. 
3. Studentid_sdlc.txt: Importance of learning DevOps in the 
software development cycle. 
Reference Steps: 
1. Create Files: (You can use any file editor or IDE) 
touch 1023756_gb.txt 1023756_devops.txt 1023756_sdlc.txt 
2. Add Content: 
o Open each file in a text editor and add the required 
information. 
3. Stage and Commit: (Put your own commit message) 
git add 1023756_gb.txt 1023756_devops.txt 1023756_sdlc.txt 
git commit -m "Add gb, devops, and sdlc information" 
4. Repeat: Ensure you make at least 10 commits, each with clear 
and descriptive messages. 
Merge their branch into the main branch. 
7. Merging Branches and Resolving Conflicts 
• Regularly pull updates from the remote repository to your local 
branches. 
• Resolve any merge conflicts that arise. 
8. Updating README.md 
Responsibilities: 
• All Members: Update the README.md to include repository details and 
group information. 
Suggested Sections: 
1. Project Title 
2. Group Members: 
o List each member with their Student ID and GitHub 
username. 
3. Project Description: 
o Brief overview of what the assignment entails. 
4. Instructions: 
o How to set up the project locally. 
5. CI/CD Details: 
o Information about the CI pipeline setup. 
6. Branching Strategy: 
o Explain the branching conventions used. 
Reference Example README.md: (Put your own details) 
# COMP2156_Group1_Assignment 
## Group Members - **Leader:** Pritesh Patel (1023756) - [GitHub](https://github.com/priteshpatel) - **Member 2:** Jane Doe (1023456) - [GitHub](https://github.com/janedoe) - **Member 3:** John Smith (1027890) - [GitHub](https://github.com/johnsmith) 
## Project Description 
This repository hosts the group assignment for COMP2156 DevOps course, focusing on 
collaborative Git workflows, branching strategies, and CI/CD integration. 
## Setup Instructions 
1. Clone the repository. 
2. Switch to your branch using `git checkout STUDENTID-Name`. 
3. Install any dependencies as listed. 
## CI/CD Pipeline 
The project utilizes GitHub Actions for continuous integration. The workflow is defined 
in `.github/workflows/ci.yml`. 
## Branching Strategy 
Each member has their own branch named `STUDENTID-Name`. All changes are 
merged into the `main` branch via Pull Requests. 
9. Creating a Pull Request Template 
• Responsibility: Only the Leader creates the PR template. 
Reference Steps: 
1. Create a .github Directory: 
mkdir .github 
2. Create the PR Template File: 
touch .github/PULL_REQUEST_TEMPLATE.md 
3. Add the Following Content to PULL_REQUEST_TEMPLATE.md: 
## Description 
Please include a summary of the changes and the related issue.  
## Type of Change - [ ] Bug fix - [ ] New feature - [ ] Documentation update 
## Checklist - [ ] My code follows the style guidelines of this project - [ ] I have performed a self-review of my code - [ ] I have commented my code, particularly in hard-to-understand areas - [ ] I have made corresponding changes to the documentation - [ ] My changes generate no new warnings - [ ] I have added tests that prove my fix is effective or that my feature works - [ ] New and existing unit tests pass locally with my changes 
4. Commit and Push the Template: 
git add .github/PULL_REQUEST_TEMPLATE.md 
git commit -m "Add Pull Request template" 
git push origin main 
Reference: Creating a pull request template 
10. Final Submission 
Create separate PDF/DOCX file for each member and submit all file 
by one member. If any member had not contributed, please mention it 
while submitting your work. 
• Repository Link: Ensure your GitHub repository is public and copy 
the link. 
• Screenshots: 
o Capture screenshots showing: 
§ Your local repository setup. 
§ Git commit history. 
§ Branch structure. 
§ CI pipeline status. 
• Submission Folder: Upload the GitHub repository link and 
screenshots to the assignment submission folder on D2L before the 
deadline. 
Additional Tips 
• Commit Often: Regular commits make it easier to track changes and 
resolve conflicts. 
• Clear Commit Messages: Use descriptive messages to explain the 
purpose of each commit. 
• Branch Naming: Stick to the naming convention to avoid confusion. 
• Regular Syncing: Frequently pull changes from main to keep your 
branch updated. 
• Review PRs: Before merging, review changes to ensure code quality 
and consistency. 
• Documentation: Keep the README.md updated to reflect the current 
state of the project. 
• Late Submission: Late submissions will not be accepted. 
Support and Communication 
• Contact for Assistance: Reach out to pritesh.patel2@georgebrown.ca or 
use the designated Slack channel for any questions or issues. 
• Collaboration: Utilize collaborative tools like GitHub Issues or Slack 
to manage tasks and resolve queries within the group. 
By following this guide, your group should be well-equipped to handle each 
component of the assignment effectively. Good luck and ensure consistent 
communication and collaboration within your group to achieve the best 
results! 
Keep In mind 
 
• ALL Commands given in the assignment documents are for reference. 
User your knowledge and expertise to use the commands. 
• No commits or file changes/upload are allowed directly on GitHub 
website. All commits must be done on local machine of each member 
should merge their branch to main/master branch 
• You can create PR/Merge code on GitHub website 
• Each member will award marks based on their contributions to the 
assignment after verification on GitHub commits logs 
• Late submission will be awarded ZERO 
 
 
Good luck with your assignment! 
 
 
