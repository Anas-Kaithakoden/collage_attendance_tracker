# everyone starts from main
git pull origin main

# create a feature branch
git checkout -b feature/login-page

# do your work locally
# git add . -> git commit -m "Implemented login API and frontend page"

# push to remote
git push origin feature/login-page

# review -> merge to main
git checkout main
git pull origin main
git merge feature/login-page

# after merge, everyone else pulls latest main before starting next feature
git checkout main
git pull origin main

