# 100 - Introduction

GitHub Pages is a website hosting service that enables you to publish content based on source code managed within a GitHub repository.

There are three ways to publish Quarto websites and documents to GitHub Pages:

- Render sites on your local machine to the docs directory, check the rendered site into GitHub, and then configure your GitHub repo to publish from the docs directory.

- Use the quarto publish command to publish content rendered on your local machine.

- Use a GitHub Action to automatically render your files (a single Quarto document or a Quarto project) and publish the resulting content whenever you push a source code change to your repository.

We’ll cover each of these methods below, but first an important pre-requisite: you need to have a Git repository on your local machine that is synced to GitHub. The URL of the published website will be derived from the combination of your username and the repository name (e.g. https://username.github.io/reponame/).

You can optionally configure a custom domain for a GitHub Pages site, but before exploring that ground you should get your site up and running with the default domain.
