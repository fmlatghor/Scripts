# Scripts
A collection of useful scripts.

## Scripts info
| Script         | Info                                                                  |
|----------------|-----------------------------------------------------------------------|
| db             | Quickly cd into specific directories using short aliases.             |
| ffconv         | Batch convert mkvs to mp4s.                                           |
| ffconv-a       | Batch convert from one format to another.                             |
| ffconv-ar      | Batch convert from one format to another without preserving metadata. |
| gpltopnm       | Convert gpl to ppm.                                                   |
| makeself       | Make self-extractable archives for *nix-likes.                        |
| matrix-decrypt | Decrypt matrix attachments that are encrypted.                        |
| matrix-upload  | Upload attachment to matrix homeserver.                               |
| mkv-cat        | Convert multiple videos into one.                                     |
| nds-banner     | Create NDS banner.bin files.                                          |
| nlzss          | Compress/decompress Nintendo's different LZSS formats.                |
| nlzss-c        | Compress Nintendo's different LZSS formats.                           |
| pa-rescan      | Rescan audio devices (pulseaudio).                                    |
| pip-upgrade    | Upgrade all pip packages.                                             |
| repack         | Completely repack an NDS rom with `ndstool`.                          |
| scanif         | Scan several documents one-by-one with SANE/CUPS.                     |
| ugrade         | Upgrade packages for every package manager.                           |
| unpack         | Completely unpack an NDS rom with `ndstool`.                          |
| yt-dl          | youtube-dl "magic" download.                                          |
| yt-mpeg        | Turn wav/cover image into a video optimised for yt.                   |

### db
"./cfg/db" contains the directories in your database. This is the file you edit, and it follows a simple syntax.
```sh
<alias-name> /path/to/dir
```
The alias name needs to be one argument...otherwise the script can't parse it.

After editing the db file, you will run "./bin/db" -- which parses the data and outputs a file to "./dat/db-c" containing your aliases in shell form. Add `source /path/to/Scripts/dat/db-c` to your shell config. After that, just remember to source your shell config and everything should work.
