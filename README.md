# zerobot
Cute pet robot using a Raspberry Pi Zero W.

# Inspiration
https://hackaday.io/project/25092-zerobot-raspberry-pi-zero-fpv-robot

# OS installation
Use rpi-image to install Raspberry OS Lite (running Buster here).
Set `wpa_applicant.conf` and empty file `ssh` at the root of the partition `boot`.
Enable the camera with `sudo raspi-config`.

# Dependencies
- virtualenv
- python3

# Run the server
## First time running
From this repo:

```
cd server
virtualenv -p python3 venv
source venv/bin/activate
pip install -r requirements.txt
```

## Run
```
python3 video_stream.py
```

# See the stream
Go to `<hostname>:8000` on a browser in the same network, while running the server on the Raspberry Pi.