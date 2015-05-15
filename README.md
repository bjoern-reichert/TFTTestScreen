# TFTTestScreen
TFTTestScreen for mini displays with a resolution of 320x240 or 480x320.

### Requires
* Hardware: For Single Board Computer with a display like Raspberry Pi with TinyLCD 3.5", Adafruit PiTFT 3.5" or Watterott RPi-Display 2.8".
* Software: python and pygame

### Install
```
$ git clone https://github.com/bjoern-reichert/TFTTestScreen.git
$ cd TFTTestScreen/
```

### Setup
```
$ nano screen_320x240.py or nano screen_480x320.py
```
Change the variables for your system: 
```
os.environ["SDL_FBDEV"] = "/dev/fb1"
os.environ["SDL_MOUSEDRV"] = "TSLIB"
os.environ["SDL_MOUSEDEV"] = "/dev/input/touchscreen"
```
### Run
```
$ python screen_320x240.py or python screen_480x320.py
```
