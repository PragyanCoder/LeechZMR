<h1 align="center">Zee Mirror</h1>


This is a Telegram Mirror/Leech Bot written in Python for mirroring files on the Internet to your Cloud Drive, based on [Mirror-Leech-Telegram-Bot](https://github.com/anasty17/mirror-leech-telegram-bot), has undergone
substantial modifications and is designed for efficiently mirroring or leeching files from the Internet to various
destinations, including Google Drive, Telegram, or any rclone-supported cloud. It is built using asynchronous
programming in Python.

<details>
    <summary><b>View Features</b></summary>

  ## Aria2c

  - Select files from a Torrent before and during download (Requires Base URL) (task option)
  - Seed torrents to a specific ratio and time (task option)
  - Netrc support (global option)
  - Direct link authentication for a specific link while using the bot (it will work even if only the username or password
    is provided) (task option)
  - Edit Global Options while the bot is running from bot settings (global option)

  ## qBittorrent

  - External access to webui, so you can remove files or edit settings. Then you can sync settings in database with sync button in bsetting
  - Select files from a Torrent before and during download using ZEE file selector (Requires Base URL) (task option)
  - Seed torrents to a specific ratio and time (task option)
  - Edit Global Options while the bot is running from bot settings (global option)

  ## Rclone

  - Transfer (download/upload/clone-server-side) without or with random service accounts (global and user option)
  - Ability to choose config, remote and path from list with or without buttons (global, user and task option)
  - Ability to set flags for each task or globally from config (global, user and task option)
  - Abitity to select specific files or folders to download/copy using buttons (task option)
  - Rclone.conf (global and user option)
  - Rclone serve for combine remote to use it as index from all remotes (global option)
  - Upload destination (global, user and task option)

  ## Sabnzbd

  - External access to web interface, so you can remove files or edit settings. Then you can sync settings in database with sync button in bsetting
  - Remove files from job before and during download using ZEE file selector (Requires Base URL) (task option)
  - Edit Global Options while the bot is running from bot settings (global option)
  - Servers menu to edit/add/remove usenet servers

  ## JDownloader

  - Synchronize Settings (global option)
  - Waiting to select (enable/disable files or change variants) before download start
  - DLC file support
  - All settings can be edited from the remote access to your JDownloader with Web Interface, Android App, iPhone App or
    Browser Extensions

  ## Yt-dlp

  - Yt-dlp quality buttons (task option)
  - Ability to use a specific yt-dlp option (global, user, and task option)
  - Netrc support (global option)
  - Cookies support (global option)
  - Embed the original thumbnail and add it for leech
  - All supported audio formats

  ## TG Upload/Download

  - Split size (global, user, and task option)
  - Thumbnail (user and task option)
  - Leech filename prefix (user option)
  - Set upload as a document or as media (global and user option)
  - Upload all files to a specific chat (superGroup/channel/private) (global, user, and task option)
  - Equal split size settings (global and user option)
  - Ability to leech split file parts in a media group (global and user option)
  - Download restricted messages (document or link) by tg private/public/super links (task option)
  - Choose transfer by bot or user session in case you have a premium plan (global, user option and task option)
  - Mix upload between user and bot session with respect to file size (global, user option and task option)
  - Upload with custom layout multiple thubnmail (global, user option and task option)

  ## Google Drive

  - Download/Upload/Clone/Delete/Count from/to Google Drive
  - Count Google Drive files/folders
  - Search in multiple Drive folder/TeamDrive
  - Use Token.pickle if the file is not found with a Service Account, for all Gdrive functions
  - Random Service Account for each task
  - Recursive Search (only with `root` or TeamDrive ID, folder ids will be listed with a non-recursive method). Based
    on [Sreeraj](https://github.com/SVR666) searchX-bot. (task option)
  - Stop Duplicates (global and user option)
  - Custom upload destination (global, user, and task option)
  - Index link support only
    for [Bhadoo](https://gitlab.com/GoogleDriveIndex/Google-Drive-Index/-/blob/master/src/worker.js)

  ### Limits
  - Storage threshold limit 
  - Leech limit
  - Clone limit
  - Rclone limit
  - Mega limits
  - Torrent limits
  - Direct download limits
  - Yt-dlp limits
  - Google drive limits
  - JDownloader limits
  - Sabnzbd limits
  - User task limits
  - User rate limiter

  ### Group Features
  - Bot DM support
  - Message filters
  - Chat restrictions
  - Stop duplicate tasks
  - Mirror/Clone log chat
  - Force subscribe module
  - Enable/Disable drive links
  - Enable/Disable leech function
  - Enable/Disable bulk link function
  - Enable/Disable multi mirror function
  - Enable/Disable torrent seeding system
  - Token system for shortners with database support
  - Shortner link bypass detection
  - Minimum average download speed limit

  ## Status

  - Download/Upload/Extract/Archive/Split/SampleVid/Seed/Clone Status
  - Status Pages for an unlimited number of tasks, view a specific number of tasks in a message (global option)
  - Interval message update (global option)
  - Next/Previous buttons to get different pages (global and user option)
  - Status buttons to get specific tasks for the chosen status regarding transfer type if the number of tasks is more than
    30 (global and user option)
  - Steps buttons for how much next/previous buttons should step backward/forward (global and user option)
  - Status for each user (no auto refresh)

  ## Mongo Database

  - Store bot settings, JDownloader settings, qBittorrent settings, Aria2c settings, Sabnzbd settings, Google Drive
    settings, Yt-dlp settings, Rclone settings, Telegram settings, and all user settings including thumbnails and all private files.
  - Store RSS data, incompleted task messages.
  - Store config.env file on first build and incase any change occured to it, then next build it will define variables
    from config.env instead of database.

  ## Torrents Search

  - Search on torrents with Torrent Search API
  - Search on torrents with variable plugins using qBittorrent search engine

  ## Archives

  - Extract splits with or without password
  - Zip file/folder with or without password
  - Decompress zst files
  - Using 7-zip tool to extract with or without password all supported types:

  > ZIP, RAR, TAR, 7z, ISO, WIM, CAB, GZIP, BZIP2, APM, ARJ, CHM, CPIO, CramFS, DEB, DMG, FAT, HFS, LZH, LZMA, LZMA2,MBR,
  > MSI, MSLZ, NSIS, NTFS, RPM, SquashFS, UDF, VHD, XAR, Z, TAR.XZ

  ## RSS

  - Based on this repository [rss-chan](https://github.com/hyPnOtICDo0g/rss-chan)
  - Rss feed (user option)
  - Title Filters (feed option)
  - Edit any feed while running: pause, resume, edit command and edit filters (feed option)
  - Sudo settings to control users feeds
  - All functions have been improved using buttons from one command.

  ## Overall

  - Docker image support for linux `amd64, arm64/v8, arm/v7`
  - Edit variables and overwrite the private files while bot running (bot, user settings)
  - Update bot at startup and with restart command using `UPSTREAM_REPO`
  - Telegraph. Based on [Sreeraj](https://github.com/SVR666) loaderX-bot
  - Mirror/Leech/Watch/Clone/Count/Del by reply
  - Mirror/Leech/Clone multi links/files with one command
  - Custom name for all links except torrents. For files you should add extension except yt-dlp links (global and user
    option)
  - Extensions Filter for the files to be uploaded/cloned (global and user option)
  - View Link button. Extra button to open index link in broswer instead of direct download for file
  - Queueing System for all tasks (global option)
  - Ability to zip/unzip multi links in same directory. Mostly helpful in unziping tg file parts (task option)
  - Bulk download from telegram txt file or text message contains links seperated by new line (task option)
  - Join splitted files that have splitted before by split(linux pkg) (task option)
  - Sample video Generator (task option)
  - Screenshots Generator (task option)
  - Ability to cancel upload/clone/archive/extract/split/queue (task option)
  - Cancel all buttons for choosing specific tasks status to cancel (global option)
  - Convert videos and audios to specific format with filter (task option)
  - Force start to upload or download or both from queue using cmds or args once you add the download (task option)
  - Shell and Executor
  - Add sudo users
  - Ability to save upload Paths
  - Name Substitution to rename the files before upload
  - Supported Direct links Generators:

  > mediafire (file/folders), hxfile.co (need cookies txt with name) [hxfile.txt], streamtape.com, streamsb.net, streamhub.ink,
  > streamvid.net, doodstream.com,
  > feurl.com, upload.ee, pixeldrain.com, racaty.net, 1fichier.com, 1drv.ms (Only works for file not folder or business
  > account), filelions.com, streamwish.com, send.cm (file/folders), solidfiles.com, linkbox.to (file/folders),
  > shrdsk.me (
  > sharedisk.io), akmfiles.com, wetransfer.com, pcloud.link, gofile.io (file/folders), easyupload.io, mdisk.me (with
  > ytdl),
  > tmpsend.com, qiwi.gg, berkasdrive.com, mp4upload.com, terabox.com (file/folders).
</details>

------

<details>
    <summary><b>Expand to see how to deploy</b></summary>

  # How to deploy?

  ## Prerequisites

  ### 1. Installing requirements:

  - Install Docker by following the [official Docker docs](https://docs.docker.com/engine/install/debian/)

  - Clone this repo:

  ```
  git clone https://github.com/Dawn-India/Z-Mirror Z-Mirror/ && cd Z-Mirror
  ```

  <details>
      <summary>Install Python and pip(for first time users)</summary>

  - For Debian based distros

  ```
  sudo apt install python3 python3-pip
  ```

  - For Arch and it's derivatives:

  ```
  sudo pacman -S docker python
  ```

  - Install dependencies for running setup scripts:

  ```
  pip3 install -r requirements-cli.txt
  ```
  </details>

  ------

  - Tutorial Video from A to Z(Outdated but still helpful):
      <p><a href="https://youtu.be/IUmq1paCiHI"> <img src="https://img.shields.io/badge/See%20Video-black?style=for-the-badge&logo=YouTube" width="150""/></a></p>

  ------

  ### 2. Setting up config file

  ```
  cp config_sample.env config.env
  ```

  - Remove the first line saying:

  ```
  _____REMOVE_THIS_LINE_____=True
  ```

  Fill up rest of the fields. Meaning of each field is discussed below. **NOTE**: All values must be filled between
  quotes, even if it's `Int`, `Bool` or `List`.
  <details>
      <summary>View Full Config</summary>

  **1. Required Fields**

  - `BOT_TOKEN`: The Telegram Bot Token that you got from [@BotFather](https://t.me/BotFather). `Str`
  - `OWNER_ID`: The Telegram User ID (not username) of the Owner of the bot. `Int`
  - `TELEGRAM_API`: This is to authenticate your Telegram account for downloading Telegram files. You can get this
    from <https://my.telegram.org>. `Int`
  - `TELEGRAM_HASH`: This is to authenticate your Telegram account for downloading Telegram files. You can get this
    from <https://my.telegram.org>. `Str`

  **2. Optional Fields**

  - `AUTHORIZED_CHATS`: Fill user_id and chat_id of groups/users you want to authorize. Separate them by space. `Int`
  - `SUDO_USERS`: Fill user_id of users whom you want to give sudo permission. Separate them by space. `Int`
  - `DATABASE_URL`: Your Mongo Database URL (Connection string). Follow
    this [Generate Database](https://github.com/Dawn-India/Z-Mirror/tree/main#generate-database) to
    generate database. Data will be saved in Database: auth and sudo users, users settings including thumbnails for each
    user, rss data and incomplete tasks. **NOTE**: You can always edit all settings that saved in database from the
    official site -> (Browse collections). `Str`
  - `USER_SESSION_STRING`: To download/upload from your telegram account if user is `PREMIUM` and to send rss. To generate
    session string use this command `python3 generate_string_session.py` after mounting repo folder for sure. `Str`. *
  
  **3. Optional APIs**
  - `FILELION_API`: Filelion api key to mirror Filelion links. Get it
    from [Filelion](https://vidhide.com/?op=my_account). `str`
  - `STREAMWISH_API`: Streamwish api key to mirror Streamwish links. Get it
    from [Streamwish](https://streamwish.com/?op=my_account). `str`
  

  **4. GDrive Tools**

  - `GDRIVE_ID`: This is the Folder/TeamDrive ID of the Google Drive OR `root` to which you want to upload all the mirrors
    using google-api-python-client. `Str`
  - `INDEX_URL`: Refer to <https://gitlab.com/ParveenBhadooOfficial/Google-Drive-Index>. `Str`
  - `IS_TEAM_DRIVE`: Set `True` if uploading to TeamDrive using google-api-python-client. Default is `False`. `Bool`
  - `STOP_DUPLICATE`: Bot will check file/folder name in Drive incase uploading to `GDRIVE_ID`. If it's present in Drive
    then downloading or cloning will be stopped. (**NOTE**: Item will be checked using name and not hash, so this feature
    is not perfect yet). Default is `False`. `Bool`
  - `DISABLE_DRIVE_LINK`: Disable drive links for all users. Default is `False`. `Bool`
  - `USE_SERVICE_ACCOUNTS`: Whether to use Service Accounts or not, with google-api-python-client. For this to work
    see [Using Service Accounts](https://github.com/Dawn-India/Z-Mirror#generate-service-accounts-what-is-service-account)
    section below. Default is `False`. `Bool`
  
  **5. qBittorrent/Aria2c/Sabnzbd**

  - `TORRENT_TIMEOUT`: Timeout of dead torrents downloading with qBittorrent and Aria2c in seconds. `Int`
  - `BASE_URL`: Valid BASE URL where the bot is deployed to use torrent web files selection. Format of URL should
    be `http://myip`, where `myip` is the IP/Domain(public) of your bot or if you have chosen port other than `80` so
    write it in this format `http://myip:port` (`http` and not `https`). `Str`
  - `BASE_URL_PORT`: Which is the **BASE_URL** Port. Default is `80`. `Int`
  - `WEB_PINCODE`: Whether to ask for pincode before selecting files from torrent in web or not. Default
    is `False`. `Bool`.
      - **Qbittorrent NOTE**: If your facing ram issues then set limit for `MaxConnections`,
        decrease `AsyncIOThreadsCount`, set limit of `DiskWriteCacheSize` to `32` and decrease `MemoryWorkingSetLimit`
        from qbittorrent.conf or bsetting command.
      - Open port 8090 in your vps to access webui from any device. username: zee, password: @Z_Mirror

  **6. Rclone**

  - `RCLONE_PATH`: Default rclone path to which you want to upload all the files/folders using rclone. `Str`
  - `RCLONE_FLAGS`: key:value|key|key|key:value . Check here all [RcloneFlags](https://rclone.org/flags/). `Str`
  - `RCLONE_SERVE_URL`: Valid URL where the bot is deployed to use rclone serve. Format of URL should be `http://myip`,
    where `myip` is the IP/Domain(public) of your bot or if you have chosen port other than `80` so write it in this
    format `http://myip:port` (`http` and not `https`). `Str`
  - `RCLONE_SERVE_PORT`: Which is the **RCLONE_SERVE_URL** Port. Default is `8080`. `Int`
  - `RCLONE_SERVE_USER`: Username for rclone serve authentication. `Str`
  - `RCLONE_SERVE_PASS`: Password for rclone serve authentication. `Str`

  **7. JDownloader**

  - `JD_EMAIL`: jdownlaoder email sign up on [JDownloader](https://my.jdownloader.org/)
  - `JD_PASS`: jdownlaoder password

  **8. MEGA Sdk**
  - `MEGA_EMAIL`: Mega email sign up on [Mega](https://mega.nz/)
  - `MEGA_PASS`: Mega password

  **9. Sabnzbd**

  - `USENET_SERVERS`: list of dictionaries, you can add as much as you want and there is a button for servers in sabnzbd settings to edit current servers and add new servers.

    ***[{'name': 'main', 'host': '', 'port': 563, 'timeout': 60, 'username': '', 'password': '', 'connections': 8, 'ssl': 1, 'ssl_verify': 2, 'ssl_ciphers': '', 'enable': 1, 'required': 0, 'optional': 0, 'retention': 0, 'send_group': 0, 'priority': 0}]***

    - [READ THIS FOR MORE INFORMATION](https://sabnzbd.org/wiki/configuration/4.2/servers)

    - **NOTE**: Enable port 8070 in your vps to access sabnzbd full web interface
    - Open port 8070 in your vps to access web interface from any device. Use it like http://ip:8070/sabnzbd/.

  **10. Update**

  - `UPSTREAM_REPO`: Your github repository link, if your repo is private
    add `https://username:{githubtoken}@github.com/{username}/{reponame}` format. Get token
    from [Github settings](https://github.com/settings/tokens). So you can update your bot from filled repository on each
    restart. `Str`.
      - **NOTE**: Any change in docker or requirements you need to deploy/build again with updated repo to take effect.
        DON'T delete .gitignore file. For more information
        read [THIS](https://github.com/Dawn-India/Z-Mirror/tree/main#upstream-repo-recommended).
  - `UPSTREAM_BRANCH`: Upstream branch for update. Default is `main`. `Str`

  **11. Leech**

  - `AS_DOCUMENT`: Default type of Telegram file upload. Default is `False` mean as media. `Bool`
  - `LEECH_SPLIT_SIZE`: Size of split in bytes. Default is `2GB`. Default is `4GB` if your account is premium. `Int`
  - `LEECH_FILENAME_PREFIX`: Add custom word to the beginning of the leeched file name/caption. `Str`
  - `LEECH_FILENAME_SUFFIX`: Add custom word to the end of the leeched file name/caption. `Str`
  - `LEECH_CAPTION_FONT` : Font style for caption. Default is `regular`. `Str`
  - `EQUAL_SPLITS`: Split files larger than **LEECH_SPLIT_SIZE** into equal parts size (Not working with zip cmd). Default
    is `False`. `Bool`
  - `MEDIA_GROUP`: View Uploaded splitted file parts in media group. Default is `False`. `Bool`.
  - `USER_TRANSMISSION`: Upload/Download by user session. Only in superChat. Default is `False`. `Bool`
  - `MIXED_LEECH`: Upload by user and bot session with respect to file size. Only in superChat. Default is `False`. `Bool`
  - `USER_LEECH_DESTINATION`: ID or USERNAME or PM(private message) to where files would be uploaded. `Int`|`Str`. Add `-100` before channel/superGroup id.
  - `NAME_SUBSTITUTE`: Add word/letter/character/sentense/pattern to remove or replace with other words with sensitive case or without. **Notes**:
    1. Seed will get disbaled while using this option
    2. Before any character you must add `\BACKSLASH`, those are the characters: `\^$.|?*+()[]{}-`
    * Example: script/code/s | mirror/leech | tea/ /s | clone | cpu/ | \[ZEE\]/ZEE | \\text\\/text/s
      - script will get replaced by code with sensitive case
      - mirror will get replaced by leech
      - tea will get replaced by space with sensitive case
      - clone will get removed
      - cpu will get replaced by space
      - [ZEE] will get replaced by ZEE
      - \text\ will get replaced by text with sensitive case
  - `METADATA_TXT`: Edit metadata of the video. `Str`
  - `META_ATTACHMENT`: Add attachment to the metadata. `Str`
  - `THUMBNAIL_LAYOUT`: Thumbnail layout (widthxheight, 2x2, 3x3, 2x4, 4x4, ...) of how many photo arranged for the thumbnail.`Str`

**12. Super Group Features**

  - `REQUEST_LIMITS`: Limit the no. of requests per user. Default is `0`. `Int`
  - `TOKEN_TIMEOUT`: Time in seconds for token timeout. Default is `0` seconds. `Int`
  - `MINIMUM_DURATOIN`: Minimum duration for the shortner links. Open your shorturl and count the minimum time to reach to the end. If a user completes the shortener faster than the minimum required time then the bot will reject his token. Default is `0` seconds. `Int`
  - `USER_MAX_TASKS`: Maximum tasks per user. Default is `0`. `Int`
  - `AUTO_DELETE_MESSAGE_DURATION`: Time in seconds for auto delete message. Default is `0` seconds. `Int`
  - `ENABLE_MESSAGE_FILTER`: Enable message filter to stop users from sending foroward messages. Default is `False`. `Bool`
  - `DELETE_LINKS`: Enable it to delete all links from the chat to avoid copyright
    issues. Default is `False`. `Bool`
  - `DM_MODE`: Enable it to allow users to receive files in DM. Default is `False`. `Bool`
  - `STOP_DUPLICATE_TASKS`: Stop duplicate tasks for all users from all bots under the same database. Default is `False`. `Bool`
  - `INCOMPLETE_TASK_NOTIFIER`: Get incomplete task messages after restart. Require database and superGroup. Default
    is `False`. `Bool`

**13. Extras**

  - `EXTENSION_FILTER`: File extensions that won't upload/clone. Separate them by space. `Str`
  - `YT_DLP_OPTIONS`: Default yt-dlp options. Check all possible
    options [HERE](https://github.com/yt-dlp/yt-dlp/blob/master/yt_dlp/YoutubeDL.py#L184) or use
    this [script](https://t.me/mltb_official_channel/177) to convert cli arguments to api options. Format: key:value|key:
    value|key:value. Add `^` before integer or float, some numbers must be numeric and some string. `str`
      - Example: "format:bv*+mergeall[vcodec=none]|nocheckcertificate:True"
  - `SET_COMMANDS`: Auto set bot commands. Default is `False`. `Bool`
  - `CMD_SUFFIX`: commands index number. This number will added at the end all commands. `Str`|`Int`
  - `DEFAULT_UPLOAD`: Whether `rc` to upload to `RCLONE_PATH` or `gd` to upload to `GDRIVE_ID`. Default is `gd`. Read
    More [HERE](https://github.com/Dawn-India/Z-Mirror/tree/main#upload).`Str`
  - `STATUS_LIMIT`: Limit the no. of tasks shown in status message with buttons. Default is `10`. **NOTE**: Recommended
    limit is `4` tasks. `Int`
  - `STATUS_UPDATE_INTERVAL`: Time in seconds after which the progress/status message will be updated. Recommended `10`
    seconds at least. `Int`
  - `DOWNLOAD_DIR`: The path to the local folder where the downloads should be downloaded to. `Str`

**14. Feature Control**
  - `DISABLE_BULK`: Disable bulk link function. Default is `False`. `Bool`
  - `DISABLE_MULTI`: Disable multi mirror function. Default is `False`. `Bool`
  - `DISABLE_SEED`: Disable torrent seeding system. Default is `False`. `Bool`
  - `DISABLE_LEECH`: Disable leech function. Default is `False`. `Bool`

**15. Chat IDs**
  - `FSUB_IDS`: Chat ID/USERNAME where force subscribe module will work. Force users to join the channel before using the
    bot. `str`
  - `LOG_CHAT_ID`: Chat ID/USERNAME where all logs will be sent. `str`
  - `DUMP_CHAT_ID`: Chat ID/USERNAME where all leeched files will be sent. `str`

**16. Limits**
  - `STORAGE_THRESHOLD`: Storage threshold limit in GB. Default is `0`. `Int`
  - `TORRENT_LIMIT`: Torrent limit in GB. Default is `0`. `Int`
  - `DIRECT_LIMIT`: Direct download limit in GB. Default is `0`. `Int`
  - `YTDLP_LIMIT`: Yt-dlp limit in GB. Default is `0`. `Int`
  - `PLAYLIST_LIMIT`: Yt-dlp playlist limit. Default is `0`. `Int`
  - `GDRIVE_LIMIT`: Google drive limit in GB. Default is `0`. `Int`
  - `MEGA_LIMIT`: Mega limit in GB. Default is `0`. `Int`
  - `LEECH_LIMIT`: Leech limit in GB. Default is `0`. `Int`
  - `CLONE_LIMIT`: Clone limit in GB. Default is `0`. `Int`
  - `RCLONE_LIMIT`: Rclone limit in GB. Default is `0`. `Int`
  - `JD_LIMIT`: JDownloader limit in GB. Default is `0`. `Int`
  - `NZB_LIMIT`: Sabnzbd limit in GB. Default is `0`. `Int`
  - `AVG_SPEED`: Minimun average download speed limit in MB(aria2/qbit). Default is `0`. `Int`

  **17. Queue System**

  - `QUEUE_ALL`: Number of parallel tasks of downloads and uploads. For example if 20 task added and `QUEUE_ALL` is `8`,
    then the summation of uploading and downloading tasks are 8 and the rest in queue. `Int`. **NOTE**: if you want to
    fill `QUEUE_DOWNLOAD` or `QUEUE_UPLOAD`, then `QUEUE_ALL` value must be greater than or equal to the greatest one and
    less than or equal to summation of `QUEUE_UPLOAD` and `QUEUE_DOWNLOAD`.
  - `QUEUE_DOWNLOAD`: Number of all parallel downloading tasks. `Int`
  - `QUEUE_UPLOAD`: Number of all parallel uploading tasks. `Int`

  **18. RSS**

  - `RSS_DELAY`: Time in seconds for rss refresh interval. Recommended `600` second at least. Default is `600` in
    sec. `Int`
  - `RSS_CHAT`: Chat ID/USERNAME where rss links will be sent. If you want message to be sent to the channel then add
    channel id. Add `-100` before channel id. `Int`|`Str`
      - **RSS NOTES**: `RSS_CHAT` is required, otherwise monitor will not work. You must use `USER_STRING_SESSION` --OR--
        *CHANNEL*. If using channel then bot should be added in both channel and group(linked to channel) and `RSS_CHAT`
        is the channel id, so messages sent by the bot to channel will be forwarded to group. Otherwise
        with `USER_STRING_SESSION` add group id for `RSS_CHAT`. If `DATABASE_URL` not added you will miss the feeds while
        bot offline.

  **19. Torrent Search**

  - `SEARCH_API_LINK`: Search api app link. Get your api from deploying
    this [repository](https://github.com/Ryuk-me/Torrent-Api-py). `Str`
      - Supported Sites:
    > 1337x, Piratebay, Nyaasi, Torlock, Torrent Galaxy, Zooqle, Kickass, Bitsearch, MagnetDL, Libgen, YTS, Limetorrent,
    TorrentFunk, Glodls, TorrentProject and YourBittorrent
  - `SEARCH_LIMIT`: Search limit for search api, limit for each site and not overall result limit. Default is zero (
    Default api limit for each site). `Int`
  - `SEARCH_PLUGINS`: List of qBittorrent search plugins (github raw links). I have added some plugins, you can remove/add
    plugins as you want. Main
    Source: [qBittorrent Search Plugins (Official/Unofficial)](https://github.com/qbittorrent/search-plugins/wiki/Unofficial-search-plugins). `List`

  **13. NOTE**

  - All variables are not written here, you can find them in [config_sample.env](https://github.com/Dawn-India/Z-Mirror/blob/main/config_sample.env)
  </details>
</details>

------

# Build and run the Zee Mirror Bot

Make sure you still inside the repo folder and installed the docker from [official Docker docs](https://docs.docker.com/engine/install/debian/).

Build And Run The bot Using docker-compose

**NOTE**: If you want to use ports other than 80 and 8080 for torrent file selection and rclone serve respectively,
change it in [docker-compose.yml](https://github.com/Dawn-India/Z-Mirror/blob/main/docker-compose.yml)
also.

- Build and run the bot:
```
sudo docker compose up --build
```

- To stop the running bot:

```
sudo docker stop <container_id>
```

- To get log from already running image bot:
  - Get the container id by running `sudo docker ps`

```
sudo docker logs <container_id> --follow
```

------

**IMPORTANT NOTES**:

1. Set `BASE_URL_PORT` and `RCLONE_SERVE_PORT` variables to any port you want to use. Default is `80` and `8080`
   respectively.

2. Check the number of processing units of your machine with `nproc` cmd and times it by 4, then
   edit `AsyncIOThreadsCount` in qBittorrent.conf.

------

<details>
    <summary><b>Extras</b></summary>

  ## Getting Google OAuth API credential file and token.pickle

  **NOTES**

  - Old authentication changed, now we can't use bot or replit to generate token.pickle. You need OS with a local browser.
    For example `Termux`.
  - Windows users should install python3 and pip. You can find how to install and use them from google or from
    this [telegraph](https://telegra.ph/Create-Telegram-Mirror-Leech-Bot-by-Deploying-App-with-Heroku-Branch-using-Github-Workflow-12-06)
    from [Wiszky](https://github.com/vishnoe115) tutorial.
  - You can ONLY open the generated link from `generate_drive_token.py` in local browser.

  1. Visit the [Google Cloud Console](https://console.developers.google.com/apis/credentials)
  2. Go to the OAuth Consent tab, fill it, and save.
  3. Go to the Credentials tab and click Create Credentials -> OAuth Client ID
  4. Choose Desktop and Create.
  5. Publish your OAuth consent screen App to prevent **token.pickle** from expire
  6. Use the download button to download your credentials.
  7. Move that file to the root of mirrorbot, and rename it to **credentials.json**
  8. Visit [Google API page](https://console.developers.google.com/apis/library)
  9. Search for Google Drive Api and enable it
  10. Finally, run the script to generate **token.pickle** file for Google Drive:

  ```
  pip3 install google-api-python-client google-auth-httplib2 google-auth-oauthlib
  python3 generate_drive_token.py
  ```

  ------

  ## Getting rclone.conf

  1. Install rclone from [Official Site](https://rclone.org/install/)
  2. Create new remote(s) using `rclone config` command.
  3. Copy rclone.conf from .config/rclone/rclone.conf to repo folder

  ------

  ## Upload

  - `RCLONE_PATH` is like `GDRIVE_ID` a default path for mirror. In additional to those variables `DEFAULT_UPLOAD` to
    choose the default tool whether it's rclone or google-api-python-client.
  - If `DEFAULT_UPLOAD` = 'rc' then you must fill `RCLONE_PATH` with path as default one or with `rcl` to select
    destination path on each new task.
  - If `DEFAULT_UPLOAD` = 'gd' then you must fill `GDRIVE_ID` with folder/TD id.
  - rclone.conf can be added before deploy like token.pickle to repo folder root or use bsetting to upload it as private
    file.
  - If rclone.conf uploaded from usetting or added in `rclone/{user_id}.conf` then `RCLONE_PATH` must start with `mrcc:`.
  - Whenever you want to write path manually to use user rclone.conf that added from usetting then you must add
    the `mrcc:` at the beginning.
  - So in short, up: has 4 possible values which is: gd(Upload to GDRIVE_ID), rc(Upload to RCLONE_PATH), rcl(Select Rclone
    Path) and rclone_path(remote:path(owner rclone.conf) or mrcc:remote:path(user rclone.conf))

  ------

  ## UPSTREAM REPO (Recommended)

  - `UPSTREAM_REPO` variable can be used for edit/add any file in repository.
  - You can add private/public repository link to grab/overwrite all files from it.
  - You can skip adding the privates files like token.pickle or accounts folder before deploying, simply
    fill `UPSTREAM_REPO` private one in case you want to grab all files including private files.
  - If you added private files while deploying and you have added private `UPSTREAM_REPO` and your private files in this
    private repository, so your private files will be overwritten from this repository. Also if you are using database for
    private files, then all files from database will override the private files that added before deploying or from
    private `UPSTREAM_REPO`.
  - If you filled `UPSTREAM_REPO` with the official repository link, then be carefull incase any change in
    requirements.txt your bot will not start after restart. In this case you need to deploy again with updated code to
    install the new requirements or simply by changing the `UPSTREAM_REPO` to you fork link with that old updates.
  - In case you you filled `UPSTREAM_REPO` with your fork link be carefull also if you fetched the commits from the
    official repository.
  - The changes in your `UPSTREAM_REPO` will take affect only after restart.

  ------

  ## Bittorrent Seed

  - Using `-d` argument alone will lead to use global options for aria2c or qbittorrent.

  ### Qbittorrent

  - Global options: `GlobalMaxRatio` and `GlobalMaxSeedingMinutes` in qbittorrent.conf, `-1` means no limit, but you can
    cancel manually.
      - **NOTE**: Don't change `MaxRatioAction`.

  ### Aria2c

  - Global options: `--seed-ratio` (0 means no limit) and `--seed-time` (0 means no seed) in aria.sh.

  ------

  ## Using Service Accounts for uploading to avoid user rate limit

  > For Service Account to work, you must set `USE_SERVICE_ACCOUNTS` = "True" in config file or environment variables.
  > **NOTE**: Using Service Accounts is only recommended while uploading to a Team Drive.

  ### 1. Generate Service Accounts. [What is Service Account?](https://cloud.google.com/iam/docs/service-accounts)

  Let us create only the Service Accounts that we need.

  **Warning**: Abuse of this feature is not the aim of this project and we do **NOT** recommend that you make a lot of
  projects, just one project and 100 SAs allow you plenty of use, its also possible that over abuse might get your
  projects banned by Google.

  > **NOTE**: If you have created SAs in past from this script, you can also just re download the keys by running:

  ```
  cd py_generators
  python3 gen_sa_accounts.py --download-keys $PROJECTID
  ```

  > **NOTE:** 1 Service Account can upload/copy around 750 GB a day, 1 project can make 100 Service Accounts so you can
  > upload 75 TB a day.

  > **NOTE:** All people can copy `2TB/DAY` from each file creator (uploader account), so if you got
  > error `userRateLimitExceeded` that doesn't mean your limit exceeded but file creator limit have been exceeded which
  > is `2TB/DAY`.

  #### Two methods to create service accounts

  Choose one of these methods

  ##### 1. Create Service Accounts in existed Project (Recommended Method)

  - List your projects ids

  ```
  cd py_generators
  python3 gen_sa_accounts.py --list-projects
  ```

  - Enable services automatically by this command

  ```
  cd py_generators
  python3 gen_sa_accounts.py --enable-services $PROJECTID
  ```

  - Create Sevice Accounts to current project

  ```
  cd py_generators
  python3 gen_sa_accounts.py --create-sas $PROJECTID
  ```

  - Download Sevice Accounts as accounts folder

  ```
  cd py_generators
  python3 gen_sa_accounts.py --download-keys $PROJECTID
  ```

  ##### 2. Create Service Accounts in New Project

  ```
  cd py_generators
  python3 gen_sa_accounts.py --quick-setup 1 --new-only
  ```

  A folder named accounts will be created which will contain keys for the Service Accounts.

  ### 2. Add Service Accounts

  #### Two methods to add service accounts

  Choose one of these methods

  ##### 1. Add Them To Google Group then to Team Drive (Recommended)

  - Mount accounts folder

  ```
  cd accounts
  ```

  - Grab emails form all accounts to emails.txt file that would be created in accounts folder
  - `For Windows using PowerShell`

  ```
  $emails = Get-ChildItem .\**.json |Get-Content -Raw |ConvertFrom-Json |Select -ExpandProperty client_email >>emails.txt
  ```

  - `For Linux`

  ```
  grep -oPh '"client_email": "\K[^"]+' *.json > emails.txt
  ```

  - Unmount acounts folder

  ```
  cd ..
  ```

  Then add emails from emails.txt to Google Group, after that add this Google Group to your Shared Drive and promote it to
  manager and delete email.txt file from accounts folder

  ##### 2. Add Them To Team Drive Directly

  - Run:

  ```
  cd py_generators
  python3 add_to_team_drive.py -d SharedTeamDriveSrcID
  ```

  ------

  ## Generate Database

  1. Go to `https://mongodb.com/` and sign-up.
  2. Create Shared Cluster.
  3. Press on `Database` under `Deployment` Header, your created cluster will be there.
  5. Press on connect, choose `Allow Access From Anywhere` and press on `Add IP Address` without editing the ip, then
    create user.
  6. After creating user press on `Choose a connection`, then press on `Connect your application`. Choose `Driver` *
    *python** and `version` **3.12 or later**.
  7. Copy your `connection string` and replace `<password>` with the password of your user, then press close.

  ------

  ## Multi Drive List

  To use list from multi TD/folder. Run driveid.py in your terminal and follow it. It will generate **list_drives.txt**
  file or u can simply create `list_drives.txt` file in working directory and fill it, check below format:

  ```
  DriveName folderID/tdID or `root` IndexLink(if available)
  DriveName folderID/tdID or `root` IndexLink(if available)
  ```

  Example:

  ```
  TD1 root https://example.dev
  TD2 0AO1JDB1t3i5jUk9PVA https://example.dev
  ```

  -----

  ## Yt-dlp and Aria2c Authentication Using .netrc File

  For using your premium accounts in yt-dlp or for protected Index Links, create .netrc file according to following
  format:

  **Note**: Create .netrc and not netrc, this file will be hidden, so view hidden files to edit it after creation.

  Format:

  ```
  machine host login username password my_password
  ```

  Example:

  ```
  machine instagram login anas.tayyar password mypassword
  ```

  **Instagram Note**: You must login even if you want to download public posts and after first try you must confirm that
  this was you logged in from different ip(you can confirm from phone app).

  **Youtube Note**: For `youtube` authentication
  use [cookies.txt](https://github.com/ytdl-org/youtube-dl#how-do-i-pass-cookies-to-youtube-dl) file.

  Using Aria2c you can also use built in feature from bot with or without username. Here example for index link without
  username.

  ```
  machine example.workers.dev password index_password
  ```

  Where host is the name of extractor (eg. instagram, Twitch). Multiple accounts of different hosts can be added each
  separated by a new line.

  -----

  >

  ## All Thanks To Our Contributors

  <a href="https://github.com/Dawn-India/Z-Mirror/graphs/contributors">
    <img src="https://contrib.rocks/image?repo=Dawn-India/Z-Mirror" />
  </a>

  ## Donations

  <p> If you feel like showing your appreciation for this project, then how about buying me a coffee.</p>

  [!["Buy Me A Coffee"](https://storage.ko-fi.com/cdn/kofi2.png)](https://ko-fi.com/anasty17)

  Binance ID:

  ```
  52187862
  ```

  USDT Address:

  ```
  TEzjjfkxLKQqndpsdpkA7jgiX7QQCL5p4f
  ```

  Network:

  ```
  TRC20
  ```
  TRX Address:

  ```
  TEzjjfkxLKQqndpsdpkA7jgiX7QQCL5p4f
  ```

  Network:

  ```
  TRC20
  ```

  BTC Address:

  ```
  17dkvxjqdc3yiaTs6dpjUB1TjV3tD7ScWe
  ```

  ETH Address:

  ```
  0xf798a8a1c72d593e16d8f3bb619ebd1a093c7309
  ```
</details>

-----
