Three places

[path]/etc/gitconfig file

Contains values applied to every user on the system and all their repositories. If you pass the option --system to git config, it reads and writes from this file specifically. 

~/.gitconfig or ~/.config/git/config file

Values specific personally to you, the user. You can make Git read and write to this file specifically by passing the --global option, and this affects all of the repositories you work with on your system.

config file in the Git directory (that is, .git/config) of whatever repository you’re currently using

Specific to that single repository. You can force Git to read from and write to this file with the --local option, but that is in fact the default.

View all of your settings and where they are coming from using:

$ git config key [--list] [--show-origin]