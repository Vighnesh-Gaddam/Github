# How to Fork and Contribute to a GitHub Repository

## 1. Fork the Repository
Forking is creating a personal copy of someone else's repository in your GitHub account.
- Go to the GitHub repository you want to contribute to.
- Click on the **Fork** button at the top right corner of the repository page. This will create a copy of the repository in your GitHub account.

## 2. Clone the Forked Repository
Once you've forked the repository, you need to clone it to your local machine to make changes.
- In your GitHub account, navigate to the forked repository.
- Click the green **Code** button and copy the HTTPS link.
- Open your terminal and run the following command:
  <git clone <URL> >
  Example:
  <git clone https://github.com/Vighnesh-Gaddam/hello.git >
  
- Navigate into the cloned repository:
  <cd repository-name >
  

## 3. Set Up an origin Remote
This allows you to sync changes from the original repository into your forked repository.
- Add the original repository as a remote called **origin**:
  <git remote add origin https://github.com/Vighnesh-Gaddam/hello.git>
  
- Verify the new origin remote:
  <git remote -v>
  
## 4. Create a New Branch
To avoid conflicts with the main codebase, always create a new branch for your changes.
- Create and switch to a new branch:
  <git checkout -b <new-branch-name>>

  Example:
  <git checkout -b feature-new-button>
  

## 5. Make Your Changes
- Make the necessary changes in your local repository (edit files, add features, fix bugs, etc.).
- After making changes, check the status of the files you’ve changed:
  <git status>
  

## 6. Commit Your Changes
- Add your changes to the staging area:
  <git add .>
  
- Commit your changes with a meaningful message:
  <git commit -m "Added a new feature">
  

## 7. Push Your Changes to GitHub
- Push the changes to your forked repository on the new branch:
  <git push origin <new-branch-name> >
  
  Example:
  <git push origin feature-new-button>
  

## 8. Create a Pull Request
- Go to your forked repository on GitHub.
- You’ll see a notification offering to compare & pull request.
- Click on **Compare & pull request**.
- Add a title and description for the changes you made.
- Review the changes and click **Create pull request**.

## 9. Syncing Fork with the Original Repository 
If the original repository has been updated, you’ll want to sync your fork to keep it up to date.
- Fetch the latest changes from the original repository:
  <git fetch origin>

- Merge the changes into your local main branch:
  <git checkout main >
  <git merge origin/main >
- Push the changes to your forked repository:
  <git push origin main >

## 10. Respond to Feedback
- Once the repository owner reviews your pull request, they may ask for changes. Address the feedback, commit changes, and push them to your branch. Your pull request will automatically update with the new changes.

After this process, the maintainer may merge your changes into the main repository!