# ms-git

git log
- git log --pretty=oneline
- git log --pretty=oneline --max-count=2
- git log --pretty=oneline --since='5 minutes ago'
- git log --pretty=oneline --until='5 minutes ago'
- git log --pretty=oneline --author=<your name>
- git log --pretty=oneline --all
- git log --all --pretty=format:"%h %cd %s (%an)" --since='7 days ago'
- git log --pretty=format:"%h %ad | %s%d [%an]" --graph --date=short

* --pretty="..." — определяет формат вывода.
* %h — укороченный хэш коммита
* %d — дополнения коммита («головы» веток или теги)
* %ad — дата коммита
* %s — комментарий
* %an — имя автора
* --graph — отображает дерево коммитов в виде ASCII-графика
* --date=short — сохраняет формат даты коротким и симпатичным

* Windows
* git config --global alias.co checkout
* git config --global alias.ci commit
* git config --global alias.st status
* git config --global alias.br branch
* git config --global alias.hist "log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short"
* git config --global alias.type 'cat-file -t'
* git config --global alias.dump 'cat-file -p'

== .gitconfig ==
[alias]
 co = checkout
 ci = commit
 st = status
 br = branch
 hist = log --pretty=format:\"%h %ad | %s%d [%an]\" --graph --date=short
 type = cat-file -t
 dump = cat-file -p

== nano ~/.bash_profile && source ~/.bash_profile
alias gs='git status '
alias ga='git add '
alias gb='git branch '
alias gc='git commit'
alias gd='git diff'
alias go='git checkout '
alias gk='gitk --all&'
alias gx='gitx --all'

alias got='git '
alias get='git '