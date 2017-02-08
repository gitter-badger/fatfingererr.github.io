github.com/fatfingererr
=====================

[![Join the chat at https://gitter.im/fatfingererr-blog/Lobby](https://badges.gitter.im/fatfingererr-blog/Lobby.svg)](https://gitter.im/fatfingererr-blog/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
this is the public repo accesible from [http://www.ffe.tw/](http://www.ffe.tw/)

Blog powered by cryogen is [https://github.com/fatfingererr/cryogen-blog](https://github.com/fatfingererr/cryogen-blog)

### Instructions to make changes
```
git clone git@github.com:fatfingererr/cryogen-blog.git your-blog
git clone git@github.com:fatfingererr/fatfingererr.github.com.git your-blog/resources/public
cd your-blog
lein ring server
.... edit your site to get new web version ....
... and push changes to both repos ....
git add . && git commit -am "WIP" && git push
cd resources/public &&  git add . && git commit -am "WIP" && git push && cd ../../

```

### .gitignore needs following line extra
```
/resources/public
```


### resources/templates/config.edn change :blog-prefix and add README.md to :resources
``` :blog-prefix      "" ```
``` :resources        ["css" "js" "404.html" "README.md"] ```
