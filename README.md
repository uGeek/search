## Install
The first option is to install the application and respond to the word **search**.

I like to use the letter **s**, which is faster

Using command the word "**s**"

```
sudo curl -L https://raw.githubusercontent.com/uGeek/search/master/search \
          -o /usr/bin/sx && sudo chmod +x /usr/bin/sx
```

## Help

```
How to use: search [OPTIONS]

sx              -> Google
sx t            -> Translation of a website with google translate
sx tt language  -> Google translate. Language = es, en, fr, it, de, ...
sx d            -> Duck Duck Go
sx b            -> Bing
sx yh           -> Yahoo
sx yd           -> Yandex
sx sp           -> StartPage
sx and          -> YouTube
sx i            -> Google Image
sx m            -> Google Maps
sx gh           -> GitHub
sx r            -> Reddit
sx rs subreddit -> SubReddit
sx w            -> Wikipedia
sx wl           -> Wallapop
sx ax           -> AliExpress
sx e            -> ebay
sx s            -> Spotify
sx dz           -> Deezer
sx trello       -> Trello
sx imdb         -> IMDB
sx -e           -> Open configuration file, to change the browser
sx -h, --help   -> Help

search v0.1 04/07/2020
 Copyright (C) 2020 Angel. uGeek
 ugeekpodcast@gmail.com
 https://ugeek.github.io
```


## Browser, Default search engine and language
The default Browser is **Firefox**, **Google** Search and the Spanish language. You can change this using the following command

To set browser terminal version, add in the configuration file variable, TERMINAL=y


```
search -e
```

## Search in the default search engine.

As simple as typing on your terminal
```
s
```
Then search will ask you what you want to search
```
Search Google:  
```

## Search YouTube

```
s y
```

## Translate text
To translate text, we have to indicate in which language we want it to be translated.
Example: Translate text into French

```
s tt fr
```
[languages allowed](https://cloud.google.com/translate/docs/languages)


## personalized
Customize with your favorite search engines or options

In the file **~/.config/search/search.engine** add them.

Also, for this search, I will add in Brave Browser

Example:

```
wl="https://es.wallapop.com/search?keywords="   # url with option. here "wl"

if [ "$MT" = "wl" ]                             # add "wl"
then
    CMD="brave-browser  $wl"                    # add "wl". if you want the default browser, change brave-browser for $BROWSER
    MOTOR="Wallapop"                            # name of engine "Wallapop"
fi
```


## Change the default search engine

Add in config file
Exem: Change the default search engine



```
#  # Utilizar buscador por defecto personalizado
#  MT=$(echo $1)
#  if [ "$1" = "" ] ; then MT=$(echo $DEFAULT) ; fi
#  
#  # SearXNG   Instance: https://searx.work/
#  sx="https://searx.work/search?q="
#  if [ "$MT" = "sx" ] ; then  CMD="$BROWSER  $sx" ;  MOTOR="SearXNG" ; fi

```





## Contact

If you want to contact me you can reach me at https://ugeek.github.io.

## License

This project uses the following license: [MIT License](https://choosealicense.com/licenses/mit/).





