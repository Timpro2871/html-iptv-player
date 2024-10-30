# html-iptv-player

## Overview

HTML IPTV Player with EPG viewer for M3U8 playlist

https://dbghelp.github.io/player.html?file=<link to playlist.m3u8\>

https://dbghelp.github.io/player.html?file=https://dbghelp.github.io/playlist.m3u8

## Features

- Mouse over channel logo to view EPG for specific channel (with thumbnail images from epg.xml)
- Click on EPG button to view EPG for all channels (Traditional EPG)
- Supports different key format (hex, base64, multiple keys)
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

## Usage

To be updated
