# 100 - Freezing Computations

To make sure that R, Python, and Julia code is only executed locally, configure your project to use Quarto’s [freeze](https://quarto.org/docs/projects/code-execution.html#freeze) feature by adding this to your ```_quarto.yml```:

```
execute:
  freeze: auto
```
_quarto.yml

Now, fully re-render your site:

```
$ quarto render
```

If you have executable code in your project you’ll notice that a ```_freeze``` directory has been created at the top level of your project. This directory stores the results of computations and should be checked in to version control. Whenever you change a ```.qmd``` file with executable code, it will automatically be re-run during your next render and the updated computations will be stored in ```_freeze```.

Note that an alternative approach is to execute the code as part of the GitHub Action. For now we’ll keep things simpler by executing code locally and storing the computations by using freeze. Then, further below, we’ll cover [Executing Code](https://quarto.org/docs/publishing/github-pages.html#executing-code) within a GitHub Action.
