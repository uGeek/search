## Install
The first option is to install the application and respond to the word **search**.

I like to use the letter **s**, which is faster

```

Using command the word "**s**"

```
sudo curl -L https://raw.githubusercontent.com/uGeek/search/master/search \
          -o /usr/bin/s && sudo chmod +x /usr/bin/s
```

## Help

```
How to use: search [OPTIONS]

s              -> Google
s t            -> Translation of a website with google translate
s tt language  -> Google translate. Language = es, en, fr, it, de, ...
s d            -> Duck Duck Go
s b            -> Bing
s yh           -> Yahoo
s yd           -> Yandex
s sp           -> StartPage
s and          -> YouTube
s i            -> Google Image
s m            -> Google Maps
s gh           -> GitHub
s r            -> Reddit
s rs subreddit -> SubReddit
s w            -> Wikipedia
s wl           -> Wallapop
s ax           -> AliExpress
s e            -> ebay
s s            -> Spotify
s dz           -> Deezer
s trello       -> Trello
s imdb         -> IMDB
s -e           -> Open configuration file, to change the browser
s -h, --help   -> Help

search v0.1 04/07/2020
 Copyright (C) 2020 Angel. uGeek
 ugeekpodcast@gmail.com
 https://ugeek.github.io
```
## Browser, Default search engine and language
The default Browser is **Firefox**, **Google** Search and the Spanish language. You can change this using the following command

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


## Contact

If you want to contact me you can reach me at https://ugeek.github.io.

## License

This project uses the following license: [MIT License](https://choosealicense.com/licenses/mit/).





