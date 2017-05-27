oh-my-zsh
======

## 主题
oh-my-zsh默认只启用git插件
编辑文件

    vim ~/.zshrc

我用的主题

    ZSH_THEME="ys"

## 插件
### 启用插件

编辑这个子段，把启用的插件都添加进去，默认只启用git，下面是我启用的插件

       plugins=(git archlinux colored-man-pages composer bower pip gem bundler ruby rake rails)

### 插件列表

这个文件的插件列表是怎么来的，当然是生成的了

    for item in $(ls ~/.oh-my-zsh/plugins) ;echo \* $item >>oh-my-zsh.md

然后我又装了一手好B

本来想写个中文插件的介绍，但感觉好像没必要，官方的足够好了

https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins-Overview

----
* adb
* ant
* apache2-macports
* arcanist
* archlinux
* asdf
* autoenv
* autojump
* autopep8
* aws
* battery
* bbedit
* bgnotify
* boot2docker
* bower
* branch
* brew
* bundler
* bwana
* cabal
* cake
* cakephp3
* capistrano
* cargo
* cask
* catimg
* celery
* chruby
* chucknorris
* cloudapp
* codeclimate
* coffee
* colemak
* colored-man-pages
* colorize
* command-not-found
* common-aliases
* compleat
* composer
* copybuffer
* copydir
* copyfile
* cp
* cpanm
* debian
* dircycle
* dirhistory
* dirpersist
* django
* dnf
* docker
* docker-compose
* dotenv
* droplr
* emacs
* ember-cli
* emoji
* emoji-clock
* emotty
* encode64
* extract
* fabric
* fancy-ctrl-z
* fasd
* fastfile
* fbterm
* fedora
* firewalld
* forklift
* fossil
* frontend-search
* gas
* gb
* geeknote
* gem
* git
* git-extras
* gitfast
* git-flow
* git-flow-avh
* github
* git-hubflow
* gitignore
* git-prompt
* git-remote-branch
* glassfish
* globalias
* gnu-utils
* go
* golang
* gpg-agent
* gradle
* grails
* grunt
* gulp
* heroku
* history
* history-substring-search
* httpie
* iwhois
* jake-node
* jhbuild
* jira
* jruby
* jsontools
* jump
* kate
* kitchen
* knife
* knife_ssh
* kubectl
* laravel
* laravel4
* laravel5
* last-working-dir
* lein
* lighthouse
* lol
* macports
* man
* marked2
* mercurial
* meteor
* mix
* mix-fast
* mosh
* mvn
* mysql-macports
* n98-magerun
* nanoc
* ng
* nmap
* node
* nomad
* npm
* nvm
* nyan
* osx
* pass
* paver
* pep8
* per-directory-history
* perl
* perms
* phing
* pip
* pj
* pod
* postgres
* pow
* powder
* powify
* profiles
* pyenv
* pylint
* python
* rails
* rake
* rake-fast
* rand-quote
* rbenv
* rbfu
* react-native
* rebar
* redis-cli
* repo
* rsync
* ruby
* rust
* rvm
* safe-paste
* sbt
* scala
* scd
* screen
* scw
* sfffe
* shrink-path
* singlechar
* spring
* sprunge
* ssh-agent
* stack
* sublime
* sudo
* supervisor
* suse
* svn
* svn-fast-info
* swiftpm
* symfony
* symfony2
* systemadmin
* systemd
* taskwarrior
* terminalapp
* terminitor
* terraform
* textastic
* textmate
* thefuck
* themes
* thor
* tig
* tmux
* tmux-cssh
* tmuxinator
* torrent
* tugboat
* ubuntu
* urltools
* vagrant
* vault
* vim-interaction
* vi-mode
* virtualenv
* virtualenvwrapper
* vundle
* wakeonlan
* wd
* web-search
* wp-cli
* xcode
* yarn
* yii
* yii2
* yum
* z
* zeus
* zsh-navigation-tools
* zsh_reload
