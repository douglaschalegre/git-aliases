With this alias, you can now use git ci commit message, and it will be expanded to git commit -m "commit message".

````shell
git config --global alias.ci '!f() { git commit -m "$*"; }; f'

````