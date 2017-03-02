#  album2mp4
Converts a folders of mp3 files into a mp4 single. Useful for uploading to youtube.
It will also generate a handy .txt file describing when the start of each track is.

## Requirements

You will need:

* Python
* `pip install mutagen`, used for analysing mp3 tags and info
* A recent version of ffmpeg or avconv 

It should work on any system as long as you have those requirements, if you're 
running windows, you will need to specify a font file path.
## Usage

You can quickly generate a file by running:

```
./album2mp4.py -f /path/to/folder -o /path/to/output.mp4 -c /path/to/folder/coverart.jpg
```

Running `album2mp4.py --help` will yield:

```
usage: album2mp4.py [-h] [-f folder] [-o output] [-c cover] [-s]
                    [-p font_path] [-v]

Turn a folder of mp3 files into a single video suitable for youtube upload

optional arguments:
  -h, --help            show this help message and exit
  -f folder, --folder folder
                        The folder containing the mp3 files
  -o output, --output output
                        The name of the output file
  -c cover, --cover cover
                        Location of the cover art
  -s, --song-title      Add the song title to the video
  -p font_path, --font-path font_path
                        Path to font file
  -v, --verbose         Provide verbose output

```