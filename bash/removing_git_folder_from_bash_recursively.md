# How to remove the .git folder recursively

Today, I learned how to remove the .git or other dot folders recursively 

 ```bash
find . | grep .git | xargs rm -rf
```

Source: [Remove all git files recursively](http://montanaflynn.me/2013/03/devops/remove-all-git-files-recursively/)

