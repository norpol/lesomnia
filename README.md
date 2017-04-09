lesomnia - Less insomnia
========================
`lesomnia` is an ugly hack I made the last minutes before going to bed, deciding I want to wake up the next day with music - played by my lovely laptop which rests next to me.

Usage (non of the arguments are optional):
```bash
./lesomnia https://www.youtube.com/watch\?v\=Fow7iUaKrq4 09:30
./lesomnia ~/Music/Artist/Album42/ 10:30
```

You can control mpv via. an ipc-socket. Example:
```bash
$ socat - UNIX-CONNECT:/tmp/mpv.socket
pause
{"event":"pause"}
pause
{"event":"unpause"}
```

Issues:
 - [x] If it's currently > 12:00, rtcwake will wakeup the next day

