# hexo-theme-future

Demo: 👍 [YulinLiang](https://yulinliang.com)  || 

## Install
```
$ git clone https://github.com/yulin-liang/hexo-theme-future.git themes/future
```

## Enable
Modify theme setting in _config.yml to future.

```
_config.yml
+ theme: future
```

## Prism syntax highlighter
- Setup:
    - Edit the `_config.yml` file in the root directory and disable the default hightlighter.
      ```
      highlight:
        enable: false
      ```
    - Add the following configuration lines in the `_config.yml`
      ```
      marked:
        langPrefix: line-numbers language-
      ```
    - Clean cache and rerun hexo server
      ```
      hexo clean && hexo s
      ```
- Advance:
    If you want to support more language or enable more features, you can download your own `prism.js` and `prism.css` in https://prismjs.com/download.html, and you just need to replace the original `source/lib/prism/prism.js` and `source/lib/prism/prism.css`.

    Please remember to clean the cache before starting hexo server.