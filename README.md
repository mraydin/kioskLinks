# Kiosk Links
> **SOLVED using Streamlink**
```
sudo apt install git python-setuptools
git clone https://github.com/streamlink/streamlink
cd streamlink/
sudo python setup.py install
```
> **then**
```
streamlink -p "omxplayer --timeout 20" --player-fifo <youtube-livestream-url> <best | worst | [resolution height]
```
 > **egg-info**
```
python setup.py install_egg_info
pip install -e .
```
---
## How to Display Images on Raspbian Command Line with fbi
 > **Install fbi**
 ```
sudo apt-get update
sudo apt-get -y install fbi
 ```
 > **Use fbi**
 ```
fbi -a myphoto.jpg
fbi -a *.jpg
fbi -a -t 5 *.jpg
 ```
 > **Command line options**
 ```
-h Print usage info.
-V Print fbi version number.
-l file Read image filelist from file.
-a Enable autozoom
-v Be verbose: enable status line on the bottom of the screen.
-u Randomize the order of the filenames.
-e Enable editing commands.
-p Preserve timestamps (when editing images).
-t sec Load next image after sec seconds without any keypress (i.e.slideshow).
-1 Don't loop (only use with -t).
-g n Gamma correction. Default is 1.0.
 ```
 ---
  > **omxplayer doesn't play audio when streaming**
  ```
youtube-dl -F <youtube-url> # print the available formats
omxplayer `youtube-dl -g -f <format_id> <youtube-url>` # play the video
```


