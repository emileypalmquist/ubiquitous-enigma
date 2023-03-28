# Git Workflow Walkthrough

- pull remote main branch changes to local main branch: `git pull origin main`
- create new branch: `git checkout -b name-of-branch`
- make changes and commit code often
  - `git add .`
  - `git commit -m "some meaningful commit message"`
  - push changes to github: `git push origin name-of-branch`
- When you are ready to merge your code into the main branch:
  - Checkout the main branch to pull changes from remote main branch
    - `git checkout main`
    - `git pull origin main`
  - checkout feature branch you want to merge with main: `git checkout name-of-branch`
  - merge local main branch into feature branch: `git merge main`
  - if there are any merge conflicts handle them.
  - push feature branch to github: `git push origin name-of-branch`
- initiate pull request on github, add reviewers, wait for pull request to be approved and merge to main on github
