# plex_top_playlists
**New Update has BREAKING changes.  Please check out settings.ini.example and adjust.**
**NOW UPDATED FOR PYTHON 3.  Python 2 not tested and will probably not be working.  MUST USE PYTHON 3 with new updates.**

A python script to get top weekly or top popular lists and put them in plex as playlists.  It will make a playlist for each user on your server.
This is my first time ever creating a python script.  Also the first time really adding something useful to GitHub

Use at your own risk.  I have it running nightly

## Read This

This script is assuming you are using "Plex Movie" as your library check.  If you are using TMDB it will not work.

The TV Shows playlists give the last episode in your library for the show.  You can easily click the show name to go to it.

The playlists can be created for any of the following
* All shared users (Normal or Managed)
* Specific users by username
* Only the script running user

## What lists this script currently retreives

* Trakt Playlists Movies
* Trakt Playlists Shows
* IMDB Chart Lists
* IMDB Custom lists
* IMDB Search Lists
* Missing Movies or Shows can be shown with relevent IDs to search in Sonarr or Radarr
* Helper commands to see relevent information or one off playlist actions

## Future wants to add (any help is welcome)

* Create/Update Collections from list (where order does not matter)
* Add Tautulli Lists
* Auto Add to Radarr
* Auto Add to Sonarr
* Tautulli history algorithim to suggest unwatched to a playlist or collection

# Getting Started

## Get plex token

**Required for everything in this script**

This page will show you where your token is

https://support.plex.tv/hc/en-us/articles/204059436-Finding-an-authentication-token-X-Plex-Token

This page will show you how to view your xml to see that link you grab your token from

https://support.plex.tv/hc/en-us/articles/201998867

### Get Trakt API key (Optional)

Used if you want to grab any Trakt playlists.  Not required.

To connect to Trakt you need to get an api key.  You can easily create one.  Here are the steps for that
1) go to Trakt.tv
2) create a user if you dont have one
3) Sign in
4) go here https://trakt.tv/oauth/applications/new
* Name - call it what you want
* Description - needed, put whatever you want
* redirect url - put any websit
* dont need anything else filled out
5) grab the Client ID to use as your Trakt API Key

# Setup Instructions in the Wiki
* [Linux](https://github.com/pbrink231/plex_top_playlists/wiki/Linux-Setup-and-Update)
* [Windows](https://github.com/pbrink231/plex_top_playlists/wiki/Windows-Setup-and-Update)


# Examples

This created a playlist for each user in plex for all found in the list.  The output shows what was not added because it was missing.

![movie list output](https://github.com/pbrink231/plex_top_playlists/wiki/images/Movie-Output-example.PNG)



# Used references to create the script

Thank you JonnyWong16 for his amazing scripts which I heavily referenced.

https://gist.github.com/JonnyWong16/2607abf0e3431b6f133861bbe1bb694e
https://gist.github.com/JonnyWong16/b1aa2c0f604ed92b9b3afaa6db18e5fd

Thank you to [gkspranger](https://github.com/gkspranger/plex_top_playlists) for forking and updating the script while I was MIA.  I heavily used his updates.


