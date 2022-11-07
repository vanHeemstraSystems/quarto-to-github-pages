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





More ...
