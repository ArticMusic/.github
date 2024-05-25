# ArticMusic

ArticMusic was made because we think that music is also part of who listens it. There is no copyright, license or economical interest that should take emotions, feelings and memories away from the people. 

This project is all about keeping safe the music you listened to, because you may want to listen again to it in the future. Yet, we encourage to [pay to support the artists](https://www.youtube.com/watch?v=7yo8av6w4sc) you like. 

In full interest of privacy, all of this software is made to be self-hosted, we do not want your data. 

The Project follows the [divide et impera](https://en.wikipedia.org/wiki/Divide_and_rule) approach, with the following structure:
- Authenticator: Easy way to extract Cookies to authenticate to services when proper API is not provided, must be paid or has strict requirements to be used
- History Extractors: Extract listening/watching history from Music/Video services
- Filter: Filter content from History Extractors, removing things that shouldn't be archived (AI-driven content-recognition to identify video content and music content)
- Identifier: Reconstruct song metadata, useful for re-uploads and remixes, identify original artist and song name in remixes/mashups. Given a song ID and a platform, allows to get IDs for other platforms, allowing for maximum quality downloads, using Downloaders
- Downloaders: Plug-in oriented way of downloading music given an ID. Black-box oriented, given an ID we get the track out at maximum available quality, no matter what happens inside.
- P2P Sharing: If enabled, allows to run in torrent-like mode, allowing others to download music from your archive. Useful when a track completely disappears in the internet, or if you want to download music at higher quality that your plugged Downloaders allow.
- P2P Central Server: Torrent Tracker, basically
- Aggregator: Web-based UI to manage settings and storage, correct Filter decisions, check system status, listen to music and so on. One interface to rule them all.

We aim to build good and lightweight software with a good ratio between code quality, code complexity, effort and expected results. 
Do not expect enterprise-grade code on an History Extractor that may break completely at every update from the service provider.
