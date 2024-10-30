# html-iptv-player

## Overview

HTML IPTV Player with EPG viewer for M3U8 playlist

https://dbghelp.github.io/player.html?file=<link to playlist.m3u8\>

https://dbghelp.github.io/player.html?file=https://dbghelp.github.io/playlist.m3u8

## Features

- Mouse over channel logo to view EPG for specific channel (with thumbnail images from epg.xml)
- Click on EPG button to view EPG for all channels (Traditional EPG)
- Supports different key formats (hex, base64, multiple keys)
- Supports DASH, HLS, MSS (using shaka player)


## Screenshots
*Channel logos used for illustration purpose only
![Local Image](./img/home.png)
![Local Image](./img/home_2.png)
![Local Image](./img/home_3.png)
![Local Image](./img/epg_all.png)
![Local Image](./img/epg_all_2.png)
![Local Image](./img/epg_all_3.png)

## Sample M3U8 playlist format
```
#EXTM3U url-tvg="https://raw.githubusercontent.com/dbghelp/StarHub-TV-EPG/refs/heads/main/starhub.xml, https://raw.githubusercontent.com/dbghelp/mewatch-EPG/refs/heads/main/mewatch.xml" refresh="3600"

#EXTINF:-1  tvg-id="532" tvg-logo="https://poster.starhubgo.com/Linear_channels2/532_1920x1080_HTV.png?w=272", Channel 1
#KODIPROP:inputstream.adaptive.license_type=clearkey
#KODIPROP:inputstream.adaptive.license_key=302f80dd411e4886bca5bb1f8018a024:15b2aaf906ebec6309d40f91289127b8
https://media.axprod.net/TestVectors/Cmaf/protected_1080p_h264_cbcs/manifest.mpd

#EXTINF:-1  tvg-id="601" tvg-logo="https://poster.starhubgo.com/Linear_channels2/601_1920x1080_HTV.png?w=272", Channel 2
#KODIPROP:inputstream.adaptive.license_type=clearkey
#KODIPROP:inputstream.adaptive.license_key={ "keys":[ { "kty":"oct", "k":"FbKq+Qbr7GMJ1A+RKJEnuA==", "kid":"MC+A3UEeSIa8pbsfgBigJA==" } ], "type":"temporary" }
https://media.axprod.net/TestVectors/Cmaf/protected_1080p_h264_cbcs/manifest.mpd

#EXTINF:-1  tvg-id="401" tvg-logo="https://poster.starhubgo.com/Linear_channels2/401_1920x1080_HTV.png?w=272", Channel 3
#KODIPROP:inputstream.adaptive.license_type=clearkey
#KODIPROP:inputstream.adaptive.license_key={ "keys":[ { "kty":"oct", "k":"FbKq+Qbr7GMJ1A+RKJEnuA==", "kid":"MC+A3UEeSIa8pbsfgBigJA==" } , { "kty":"oct", "k":"FbKq+Qbr7GMJ1A+RKJEnuA==", "kid":"MC+A3UEeSIa8pbsfgBigJA==" } ], "type":"temporary" }
https://media.axprod.net/TestVectors/Cmaf/protected_1080p_h264_cbcs/manifest.mpd
```
## Test out your epg.xml

https://github.com/dbghelp/html-epg-viewer

https://dbghelp.github.io/epg.html?file=<link to epg.xml\>

[https://dbghelp.github.io/epg.html?file=https://raw.githubusercontent.com/dbghelp/mewatch-EPG/refs/heads/main/mewatch.xml](https://dbghelp.github.io/epg.html?file=https://raw.githubusercontent.com/dbghelp/mewatch-EPG/refs/heads/main/mewatch.xml)

## Create your own IPTV web app in 5 minutes

1. Download `create_your_own_iptv_webapp.html` from this repository
2. Open the file in notepad, search for `m3u8Link='https://dbghelp.github.io/playlist.m3u8` and replace the hardcoded playlist.m3u8 link to your m3u8 playlist link
3. Rename the file to what you like
4. Find a static html hosting service and upload the html file (or use python -m http.server to host locally)

## CORS issue

Here's a few ways to solve it:
- Try to use incognito mode (may work)
- Find a web browser extension for this
- Use a CORS proxy
- Use other alternative links

## Usage

To be updated
