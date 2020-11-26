# lastfm_utils
Utilities for communicating with Last.fm

*Note: if you want the output in a file, use output redirection: `./example > file.txt`*

### lastfm_history
```
#---------------------------------------------------------------------------
#  Description   : Get a user's listening history from Last.fm
#  Setup         : chmod +x lastfm_history
#                  export LASTFM_API_KEY=xxxxxxx
#                      - or just hardcode the API key into the program
#                      - https://www.last.fm/api/account/create
#
#  Usage         : ./lastfm_history -u USRN
#  Dependencies  : python3
#---------------------------------------------------------------------------
```
```
usage: lastfm_history [-h] [-d] [-p] [-t] [-w W] [-l L] -u USRN

optional arguments:
  -h, --help            show this help message and exit
  -d, --date            display tracks organized by date in JSON format
  -p, --plaintext       display date output in plaintext
  -t, --top             display top tracks (rather than recent)
  -w W, --width W       tab width for display
  -l L, --limit L       limit the number of songs
  -u USRN, --user USRN  lastfm username
```

### lastfm_covers
```
#---------------------------------------------------------------------------
#  Description   : Generate an HTML file with album art for a user's tracks
#  Setup         : chmod +x lastfm_covers
#                  export LASTFM_API_KEY=xxxxxxx
#                      - or just hardcode the API key into the program
#                      - https://www.last.fm/api/account/create
#
#  Usage         : ./lastfm_covers -u USRN
#  Dependencies  : python3, requests (https://requests.readthedocs.io/en/master/)
#---------------------------------------------------------------------------
```
```
usage: lastfm_covers [-h] [-t] [-n] [-l L] [-s S] -u USRN

optional arguments:
  -h, --help            show this help message and exit
  -t, --top             display top tracks (rather than recent)
  -n, --nohtml          display image URLs in plaintext
  -l L, --limit L       limit the number of tracks
  -s S, --size S        size of each image (S, M, L, XL)
  -u USRN, --user USRN  lastfm username
```
