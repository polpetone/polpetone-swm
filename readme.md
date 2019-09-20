# polpetone-swm - Polpetone Shell Webpage Manager

Collecting webpages in a simple yaml file and calling them from shell.

## Config Files
* initial call of this tool will create two files at ~/.polpetone-swm
    * __config.yml:__ you can change here the browser to use, default is chromim
    * __webpages.yml:__ file the webpages are saved 

## Sample Setup 
* alias webadd="vim $HOME/.polpetone-swm/webpages.yml"
* __sample call__: `webadd` -> will open webpages.yml in vim, add a new page, save and closed it.
* cp polpetone-swm $HOME/bin/web
* __sample call__: `web github` -> will open github.com and github.com/polpetone


## How it works

__sample webpages.yml file__
```
search-engine:
    - https://google.de
    - https://duckduckgo.de
    - https://yandex.ru

sport:
    - https://sport1.de
    - https://kicker.de
```

* `web sport`: Will open sport1 and kicker webpage in your configured browser
* `web search-engine`: Will open google, duckduckgo and yandex in your configured browser

* `web something`: "something" is not in `webpages.yml`, in this case the tool will 
search for "something" at google and duckduckgo and open the results in your configured browser.
