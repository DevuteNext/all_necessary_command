# Git Commands




## Fix Permission After SSH Key Change

fix project permission after ssh key change.type the command exactly as it is (with extra spaces and one dot at the end)


```bash
  sudo chown -R "${USER:-$(id -un)}" .
```
    
## StackOverflow

https://stackoverflow.com/questions/6448242/git-push-error-insufficient-permission-for-adding-an-object-to-repository-datab
