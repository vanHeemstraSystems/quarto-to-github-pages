# 100 - Private Sites

If you are publishing to a private (i.e. password protected) website then the logic within ```quarto publish``` that waits for your site to be available before opening a browser won’t work correctly. In this case you should pass the ```--no-browser``` option to bypass this:

```
$ quarto publish gh-pages --no-browser
```
