# painful-oneliners
Pull requests recommended, eye bleach too

### Unzip all password protected zip files in a directory and make a directory for each ones contents     
```bash
for file in *.zip; do mkdir "${file%.zip}"; unzip -d -P hackthebox "${file%.zip}" "$file"; done    
```

### Pull a youtube video with youtube-dl and watch it locally with mplayer or vlc     
```bash
mplayer -fs -quiet $(youtube-dl -g -f mp4 "https://www.youtube.com/watch?v=dQw4w9WgXcQ")
```
