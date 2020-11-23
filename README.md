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
usage: lastfm_history [-h] [-d] [-j] [-w W] [-l L] -u USRN

optional arguments:
  -h, --help            show this help message and exit
  -d, --date            display tracks organized by year and month
  -j, --json            display output in json format)
  -w W, --width W       tab width for display
  -l L, --limit L       limit the number of songs
  -u USRN, --user USRN  lastfm username
```
