# polpetone-swm - Polpetone Shell Webpage Manager

Collecting webpages in simple yaml file and calling them from shell.

## Config Files
* initial call will create config files at ~/.polpetone-swm

## Integration to your setup
* make an alias or sim link in your preferred bin directory

## How it works
* all bookmarks a saved and get handled in a yaml file

## Sample Setup 
* alias webadd="vim $HOME/.polpetone-swm/webpages.yml"
* __sample call__: `webadd` -> will open webpages.yml, add a new page and save and closed it.
* cp polpetone-swm $HOME/bin/web
* __sample call__: `web github` -> will open github.com and github.com/polpetone
