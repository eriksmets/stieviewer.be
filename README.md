# stieviewer.be
Stieviewer.be - unofficial online website for TV streaming using the Stievie API.

Stieviewer.be offers the possibility to watch online TV using your existing stievie subscription. This way you're no longer limited to your phone or tablet, but you can also watch online on your computer.

Demo online:
http://www.stieviewer.be/
http://play.stieviewer.be/

Please note that the demo site only allows SD streaming, while the code on the repo will stream in HD.

**Requirements:**

Google Chrome. Firefox works too, except the player which doesn't work properly right now.

A proxy server.
Due to Cross-origin limitations, video can't be loaded directly from the stievie servers.
The Stievie instance takes 2 constructor parameters. The first is a proxy host for the API calls, the second one is a proxy for video. A partial Nginx vhost configuration is located under vhost-example.conf.
It is important that the playlist proxy is located at the root of a domain! This is required for playing m3u8 files, which contain relative url's.
