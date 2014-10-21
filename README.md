mpris-ctrl
==========

Command-line utility for controlling media players supporting MPRIS (vlc, audacity, bmp, xmms2, spotify (partial), etc.)


## About
`mpris-ctrl` simplifies common `D-Bus` message commands that are supported by the [MPRIS D-Bus interface specification](http://specifications.freedesktop.org/mpris-spec/latest/)

## Installing
`mpris-ctrl` is a standalone script, and is installed by placing it (or symlinking to) somewhere in the `PATH` variable.

A suggested way to download and install for all users:
```
sudo git clone https://github.com/swarminglogic/mpris-ctrl.git /opt/mpris-ctrl
sudo ln -s /opt/mpris-ctrl/mpris-ctrl.sh /usr/local/bin/mpris-ctrl
```


## Examples

Listing active and supported MPRIS player targets:
```
$ mpris-ctrl -l
```

Toggling spotify play-pause:
```
$ mpris-ctrl spotify play-pause
```

Jump to next spotify track:
```
$ mpris-ctrl spotify next
```

Append video to vlc playlist:
```
$ mpris-ctrl vlc add-track video.mp4
```


## License
The `mpris-ctrl` utility is licensed under the MIT License.

See [`LICENSE`](LICENSE)
