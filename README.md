AR&TREx
========
AR&TREx is an artist and tracks recommendation explorer. It is an extension of the application [artist explorer](https://github.com/fsahin/artist-explorer) developed by [fshain](https://github.com/fsahin).

It excludes the explorer of related artists depending on the genre and includes tracks recommendation (using a track as a seed). It also includes a new element that allows to see the main information about the recommended tracks.

Artist Explorer
===============

See Artist Explorer at [artistexplorer.spotify.com](https://artistexplorer.spotify.com/)

Artists Explorer is a tool that helps serious music enthusiasts explore artist relationships and discover new music. Start from any artist and quickly navigate through trees of related artists, previewing their music as you go.

The app pulls related artist information from Spotify and additional data (genre, biography) from the Echo Nest. Have a look at the documentation of these APIs at:

* [https://developer.spotify.com/web-api/](https://developer.spotify.com/web-api/)
* [https://developer.echonest.com/docs/v4](https://developer.echonest.com/docs/v4)

Running Locally
===============
**Not necessary but strongly suggested:** Create a [virtualenv] (http://docs.python-guide.org/en/latest/dev/virtualenvs/) or use an existing one before installing dependencies of this project.


Echo Nest API calls are proxied through a flask server. You need to start the server first.

```
cd server
pip install -r requirements.txt
python server.py
```

And you also need to serve the files at the root of the project. You can use SimpleHTTPServer module in python. To do that, change directyory to the project base and enter the following command:
```
python -m SimpleHTTPServer
```

App
===
<img src="./img/ScreenShot.png" width="750px"/>

Consumed Libraries:
--------------
* [d3](http://d3js.org/)
* [Google Gauge Charts](https://developers.google.com/chart/interactive/docs/gallery/gauge)
* [Spotify Web API Wrapper](https://github.com/JMPerez/spotify-web-api-js)
* [geoplugin](http://www.geoplugin.com/)
* [freegeoip](https://freegeoip.net)
