# KubeBuild Demo

### Steps:

- Create a new feature branch from develop:

    git checkout -b feature/new_feature develop

- Make changes to the code (for example, modifiy the `homepage.html` file).
- Commit and push your changes.
- Bring your branch up-to-date in case other features have been merged into develop beforehand:

    git fetch && git merge develop

- After resolving the conflicts (if any), make a last push.
- Create a PR to merge the feature branch into develop. After creating the pull request, a CI build will
run with the code from the feature branch.
- After merging, another CI build will run with the updated code from develop.
- Create a PR to merge the develop branch into master. After creating the pull request, a CI build will run 
with the code from develop.
- After merging, a CI/CD build will run with the code from master.


