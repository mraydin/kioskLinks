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

