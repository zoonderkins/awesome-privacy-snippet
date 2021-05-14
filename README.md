# awesome-privacy-snippet
A collection of awesome command or snippet which enchanced our data hygine 


## Mac OSX

### Clear clipboard

`sudo nano /usr/local/bin/pbclear` & `sudo chmod +x pbclear` & `pbclear 60 &` *60 for every 60 seconds clear clipboard*

```bash
#!/bin/sh
# pbclear [seconds]

S=${1:-10}

while true
do
    pbcopy < /dev/null
    sleep $S
done
```

Source: [Stack overflow](https://apple.stackexchange.com/questions/245067/clear-clipboard-on-os-x-after-n-seconds)
