# Elan Nurhaliza — AI & Machine Learning Portfolio

This repository contains a simple static dashboard/portfolio site (HTML/CSS).

How to push & deploy

1) Initialize git, commit, and create `main` branch:

```bash
git init
git add .
git commit -m "Initial commit: portfolio"
git branch -M main
```

2) Create a remote repo and push (option A — with GitHub CLI):

```bash
gh repo create <USERNAME>/<REPO> --public --source=. --remote=origin --push
```

Option B — create repo on github.com and then:

```bash
git remote add origin https://github.com/<USERNAME>/<REPO>.git
git push -u origin main
```

3) Deployment

The repository includes a GitHub Actions workflow (`.github/workflows/deploy-pages.yml`) that publishes the repository root to GitHub Pages when you push to `main`. After the first successful workflow run, your site will be available at `https://<USERNAME>.github.io/<REPO>/` (or at `https://<USERNAME>.github.io/` if you create a repository named `<USERNAME>.github.io`).

If Pages is not already enabled, the Actions workflow will publish the site automatically; otherwise, check the repository Settings → Pages to confirm the source and URL.

Need me to create the GitHub repo and push for you? I can prepare everything here but cannot authenticate to your GitHub account — you'll need to run the `gh` or `git` commands above locally or provide a personal access token if you want me to perform the push from this environment.
