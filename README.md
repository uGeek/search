# search
Search the internet for what you want from the terminal


## Install
The first option is to install the application and respond to the word **search**.

I like to use the letter **s**, which is faster

Using command the word "**search**"

```
sudo curl -L https://raw.githubusercontent.com/uGeek/search/master/search \
          -o /usr/bin/search && sudo chmod +x /usr/bin/search
```

Using command the word "**s**"

```
sudo curl -L https://raw.githubusercontent.com/uGeek/search/master/search \
          -o /usr/bin/s && sudo chmod +x /usr/bin/s
```

## Help

```
How to use: search [OPTIONS]

search              -> Google
search t            -> Translation of a website with google translate
search tt language  -> Google translate. Language = es, en, fr, it, de, ...
search d            -> Duck Duck Go
search b            -> Bing
search yh           -> Yahoo
search yd           -> Yandex
search sp           -> StartPage
search and          -> YouTube
search i            -> Google Image
search m            -> Google Maps
search gh           -> GitHub
search r            -> Reddit
search rs subreddit -> SubReddit
search w            -> Wikipedia
search e            -> ebay
search s            -> Spotify
search dz           -> Deezer
search trello       -> Trello
search imdb         -> IMDB
search -e           -> Open configuration file, to change the browser
search -h, --help   -> Help

search v0.1 04/07/2020
 Copyright (C) 2020 Angel. uGeek
 ugeekpodcast@gmail.com
 https://ugeek.github.io
 ```
## Browser and Default search engine
The default Browser is **Firefox** and **Google** Search. You can change this using the following command

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
(languages allowed)[https://cloud.google.com/translate/docs/languages]


## Contact

If you want to contact me you can reach me at https://ugeek.github.io.

## License

This project uses the following license: [MIT License](https://choosealicense.com/licenses/mit/).





