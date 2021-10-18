# Testing Bookdown website deployment

This project used this repository as a template: https://bookdown.org/yihui/bookdown-demo/,
then generally followed [this article](https://medium.com/@delucmat/how-to-publish-bookdown-projects-with-github-actions-on-github-pages-6e6aecc7331e) to create the GitHub action to deploy as a website.

Things I changed to `.github/workflow/deploy_bookdown.yml`:
- changed the branch identified at the top of the file from `main` to `master`
- updated last section, "Deploy to GitHub Pages":
  - newer version of `Cecilapp/GitHub-Pages-deploy`
  - `GH_TOKEN` to `GITHUB_TOKEN`
  - moved `BUILD_DIR` from `env` to `with`

Also note that when creating your personal access token,
you need to select the box net to `workflow` to provide appropriate permissions.
