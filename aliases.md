With this alias, you can now use git ci commit message, and it will be expanded to git commit -m "commit message".

````shell
git config --global alias.ci '!f() { git commit -m "$*"; }; f'
````

This alias provides a visually appealing and informative log output, with colored elements for better distinction between different parts of the log entry. Useful for quickly checking a branch history instead of standard git log wich i find bloated for this pourpuse.
````shell
git config --global alias.betterlog "log --name-status --color --pretty=format:'%C(magenta)%d%n %C(yellow)%h%Creset · %C(green)%cn%Creset%n %C(cyan)%s'"
````