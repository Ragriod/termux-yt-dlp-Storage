# termux-yt-dlp

Bash script to setup yt-dlp in Termux

## How to install

1. Install [Termux from F-Droid](https://wiki.termux.com/wiki/Installing_from_F-Droid). Termux from Google Play [has](https://github.com/termux/termux-app/issues/2067) [some](https://www.reddit.com/r/termux/comments/msn5rr/pkg_update_fails/) [problems](https://stackoverflow.com/questions/67647518/i-want-to-ask-how-to-fix-this-termux-repository/68881710#68881710) with `pkg update` and will be removed in the future. You don't need root to install F-Droid application. Just allow installing from apk file.

   Even if you download from F-Droid there are some rouge repo which doesn't allows you to install the packages.
   So Open termux then type the following
```bash
$ pkg remove game-repo
$ pkg remove science-repo
$ pkg update
```
2. Now install YT-DLP

```bash
$ pkg update
$ pkg install git
$ git clone https://github.com/Ragriod/termux-yt-dlp-Storage.git
$ cd termux-yt-dlp-Storage
$ bash install.sh
```

3. Enable Termux [popup over other applications](https://bubble.dynalogix.eu/enable-display-pop-up-windows-on-new-xiaomi-phones/):

- `Long press Termux icon > i > Other permissions > Display pop-up window`
- or `Settings > Apps > Manage Apps > Termux > Other permissions > Display pop-up window`.

## Upgrade yt-dlp

Open Termux and run

`pip install -U yt-dlp`

## How to use

1. Now go into youtube (or twitter, or reddit, [full list](https://ytdl-org.github.io/youtube-dl/supportedsites.html)), watch a video, tap the share button, then tap termux and wait for the download.
2. Go into `~/storage/Download` with your file explorer and watch your downloaded video.
