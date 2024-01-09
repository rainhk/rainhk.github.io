---
layout: post
title:  "Ruby configuration"
date:   2024-01-08 21:04:50 +0530
categories: Terminal
---
Jekyll Ruby configuration


Install specific Ruby version
```javascript
$ rbenv install 3.3.3
```

Set specific Ruby version globally
```javascript
$ rbenv global 3.3.3
```

Check installed Ruby versions
```javascript
$ rbenv versions
```

Check using Ruby version
```javascript
$ ruby -v
```

Rehash needed after installing new Ruby version
```javascript
$ rbenv rehash
```



For the permission error...

Check path with which command
```javascript
$ which ruby
/usr/bin/ruby 

$ which gem
/usr/bin/gem 
```


If the path is set to above, then run following command line on the terminal
```javascript
[[ -d ~/.rbenv  ]] && \
  export PATH=${HOME}/.rbenv/bin:${PATH} && \
  eval "$(rbenv init -)"
```



Check the path if it became rbenv
```javascript
$ which ruby
/Users/username/.rbenv/shims/ruby

$ which gem
/Users/username/.rbenv/shims/gem
```
<!--Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].-->
<!---->
<!--[jekyll-docs]: https://jekyllrb.com/docs/home-->
<!--[jekyll-gh]:   https://github.com/jekyll/jekyll-->
<!--[jekyll-talk]: https://talk.jekyllrb.com/-->
