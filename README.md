# lastfm_utils
Utilities for communicating with Last.fm

### lastfm_history
```
#---------------------------------------------------------------------------
#  Description   : Get a user's listening history from Last.fm
#  Setup         : chmod +x lastfm_history
#                  export LASTFM_API_KEY=xxxxxxx
#                      - or just hardcode the API key into the variable
#                      - https://www.last.fm/api/account/create
#
#  Usage         : ./lastfm_history -u USER
#  Dependencies  : python3
#---------------------------------------------------------------------------
```
```
usage: lastfm_history [-h] [-d] [-j] [-w WIDTH] -u USER

optional arguments:
  -h, --help            show this help message and exit
  -d, --date            display tracks organized by year and month
  -j, --json            display output in json format
  -w WIDTH, --width WIDTH
                        tab width for display
  -u USER, --user USER  lastfm username
```
