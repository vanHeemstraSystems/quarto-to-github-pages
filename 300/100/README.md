# 100 - Render to docs

The simplest way to publish using GitHub Pages is to render to the ```docs``` directory and then check that directory into your repository. If you prefer not to check rendered output into version control see the discussion of using [Publish Command](https://quarto.org/docs/publishing/github-pages.html#publish-command) below.

To get started, change your project configuration to use ```docs``` as the ```output-dir```. For example:

```
project:
  type: website
  output-dir: docs
```
_quarto.yml




More ...
