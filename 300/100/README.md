# 100 - Render to docs

The simplest way to publish using GitHub Pages is to render to the ```docs``` directory and then check that directory into your repository. If you prefer not to check rendered output into version control see the discussion of using [Publish Command](https://quarto.org/docs/publishing/github-pages.html#publish-command) below.

To get started, change your project configuration to use ```docs``` as the ```output-dir```. For example:

```
project:
  type: website
  output-dir: docs
```
_quarto.yml

Then, add a ```.nojekyll``` file to the root of your repository that tells GitHub Pages not to do additional processing of your published site using Jekyll (the GitHub default site generation tool):

Mac/Linux:
```
$ touch .nojekyll
```

Windows:
```
copy NUL .nojekyll
```

Now, render your site and push it to GitHub:

```
$ quarto render
$ git push
```

Finally, configure your GitHub repository to publish from the ```docs``` directory of your ```main``` branch:

<img width="1159" alt="gh-pages-docs-dir" src="https://user-images.githubusercontent.com/1499433/200272915-ac5a255d-874c-4db0-91ca-e713afc5d691.png">

Once you’ve made this configuration change GitHub will trigger a deployment of your website. Your site will also be updated whenever you commit and push to ```main```.
