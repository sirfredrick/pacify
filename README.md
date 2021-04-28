# Pacify

> Shell script that extracts YouTube video audio and condenses it for passive language listening

Pacify downloads YouTube audio via `youtube-dl` and condenses it for a better passive listening experience.

POSIX compliant\*
\*Require `youtube-dl`(`python`), `ffmpeg`, and `dos2unix` to be installed and in the `PATH`.
Make sure that a symlink of `python3` to `python` is made

```sh
ln -s /usr/local/bin/python3 /usr/local/bin/python
```

and that `youtube-dl` is the latest version (monthly release).

```sh
youtube-dl --version
```

This script has been tested on Ubuntu 20.04, Alpine 3.13.5, FreeBSD 12.2, and OpenBSD 6.8.

## Running

```sh
chmod +x ./pacify
```

```sh
./pacify SuperTuxCart uWO5DISzMUA es
```

**Note: This video might not work on OpenBSD, try the video you want instead**

The command format is

```sh
pacify [file/directory name] [YouTube video ID] [subtitle language ID]
```

## Developing

Make sure you are using a POSIX OS and that `git` is installed and on your path then run

```sh
git clone https://github.com/sirfredrick/pacify.git
```

then follow the above steps for running it.

## Contributing

If you'd like to contribute, please fork the repository and use a feature  
branch. Pull requests are warmly welcome.

## Links

* Repository: [https://github.com/sirfredrick/pacify](https://github.com/sirfredrick/pacify)
* Issue tracker: [https://github.com/sirfredrick/pacify/issues](https://github.com/sirfredrick/pacify/issues)
* Related projects:
    * Thanks to [ffmpeg](https://ffmpeg.org/) and [youtube-dl](https://yt-dl.org/) for being pillars of the FOSS community when it comes to video/audio parsing.
    * Thanks to [shellhaters](https://shellhaters.org) for an easy to understand explanation of the POSIX standard.
    * Thanks to [Refold](https://refold.la) for a language learning guide that inspired me to write this program. See the [passive listening section](https://refold.la/roadmap/stage-1/a/passive-listening) for more details.

## License
Copyright © 2021 Sir Fredrick

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License along
with this program; if not, write to the Free Software Foundation, Inc.,
51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA. 
