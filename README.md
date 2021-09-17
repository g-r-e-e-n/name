# VideoPlayerBot
Telegram bot to stream videos in telegram voicechat for both groups and channels. Supports live strams, YouTube videos and telegram media.

## Config Vars:
### Mandatory Vars
1. `API_ID` : Get From [my.telegram.org](https://my.telegram.org/)
2. `API_HASH` : Get from [my.telegram.org](https://my.telegram.org)
3. `BOT_TOKEN` : [@Botfather](https://telegram.dog/BotFather)
4. `SESSION_STRING` : [Generate session string](https://replit.com/@ErichDaniken/Generate-Telegram-String-Session/)
5. `CHAT` : ID of Channel/Group where the bot plays Music.
### Optional Vars
1. `LOG_GROUP` : Group to send Playlist, if CHAT is a Group()
2. `ADMINS` : ID of users who can use admin commands.
3. `STARTUP_STREAM` : This will be streamed on startups and restarts of bot. You can use either any STREAM_URL or a direct link of any video or a Youtube Live link. You can also use YouTube Playlist.Find a Telegram Link for your playlist from [PlayList Dumb](https://telegram.dog/DumpPlaylist) or get a PlayList from [PlayList Extract](https://telegram.dog/GetAPlaylistbot). The PlayList link should in form `https://t.me/DumpPlaylist/xxx`.
4. `REPLY_MESSAGE` : A reply to those who message the USER account in PM. Leave it blank if you do not need this feature. 
5. `ADMIN_ONLY` : Pass `Y` If you want to make /play command only for admins of `CHAT`. By default /play is available for all.



## Requirements
- Python 3.8 or Higher.
- [FFMpeg](https://www.ffmpeg.org/).



## Deploy to Heroku

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/akhilbaiju/VideoPlayerBot)

## Deploy to VPS

```sh
git clone https://github.com/akhilbaiju/VideoPlayerBot
cd VideoPlayerBot
pip3 install -r requirements.txt
# <Create Variables appropriately>
python3 main.py
```

## Features

- Playlist, queue.
- Supports Play from Youtube Playlist.
- Change VoiceChat title to current playing song name.
- Supports Live streaming from youtube
- Play from telegram file supported.
- Starts Radio after if no songs in playlist.
- Automatically downloads audio for the first two tracks in the playlist to ensure smooth playing
- Automatic restart even if heroku restarts.
- Support exporting and importing playlist.

## LICENSE

- [GNU General Public License](./LICENSE)


## CREDITS

- [py-tgcalls](https://github.com/pytgcalls/pytgcalls)
- [Dan](https://github.com/delivrance) for [Pyrogram](https://github.com/pyrogram/pyrogram)


