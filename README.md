# qutebrowser-userscripts
Qutebrowser userscripts

## Config basics


### Spawn with URL
config.bind('x', 'spawn l<COMMAND> -u {url}')
  
  
  
### Spawn with hitnl url
config.bind('X', 'hint links spawn <COMMAND> -u {hint-url}')



### Search enginees
c.url.searchengines['a'] = 'https://wiki.archlinux.org/?search={}'
c.url.searchengines['g'] = 'http://www.google.com/search?hl=en&source=hp&ie=ISO-8859-l&q={}'
c.url.searchengines['y'] = 'https://www.youtube.com/results?search_query={}'
c.url.searchengines['gh'] = 'https://github.com/search?q={}&type=Code'

# aliases
c.aliases['gb'] = 'open -t http://bitbucket.jasonwryan.com'
c.aliases['ge'] = 'open -t https://wiki.archlinux.org/index.php/Forum_Etiquette'


config.bind('x', 'spawn l<COMMAND> -u {url}')
  
config.bind('X', 'hint links spawn <COMMAND> -u {hint-url}')



### TOR network togler
```
config-cycle -p content.proxy socks://localhost:9050/ system 
```
