# Project Setup: Connecting Posit Cloud to Your Team Repo

## Initial Setup (all team members)

In the Terminal tab:

```
git init .
git config user.name "Your Name"
git config user.email "Your Email"
git config credential.helper store
git remote add origin HTTPS_URL
git remote add upstream https://github.com/Datasci-306-Project-1-Group/datasci306_wn25_project1
```

Replace `HTTPS_URL` with your team's GitHub repo URL.

## One Team Member Only

Pull the starter materials and push them to your team repo:

```
git pull upstream main
git branch -m main
git push origin main
```

When prompted: username is your **GitHub username** (not email), password is your **PAT**.

## All Other Members

After the above is done, pull from the team repo:

```
git pull --set-upstream origin main
git branch -M main
```

## Ongoing Workflow

```
git pull origin main
# edit, add, commit
git push origin main
```
