# umagiplayer
QML frontend to Clementine Music Player for Raspberry Pi with touchscreen

# Objective
Create a dedicated, standalone and connected music player based on Clementine and Raspberry Pi.

The aim is to house a Raspberry Pi 4 with touchscreen, SSD drive and rotary encoder
control knob into a HiFi component form factor, maybe as follows:

![UMAGI-MusiCore2](https://github.com/diracsbracket/umagiplayer/assets/13051119/8a3429f1-4257-4a73-ad7d-acc8a125e579)

The desktop Clementine UI is replaced by a QML-based version suitable for an embedded system with a small 800 x 480 touchscreen.

# Current status
QML files have been created that provide basic Clementine functionality such as:
* Playback control
* File browsing
* Playlist
* Library
* Album Art
* Internet: Icecast and Radio-Browser.info
* Basic player settings
* Audio control: Balance, Volume, Equalizer. Added Compressor
* Analyzer: Bar, Block, Boom, Turbine
* From a previous version of Clementine, we also included
Radio-Browser.info

In addition, the following non-Clementine features were added:
* Audio Compressor
* VU meter Analyzer option
* Performance Monitor for the Pi4

# QML interface
## Main screen

<img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/b6ae0049-8f0b-4c19-9215-aaec6b1c20e6" width=45% />

## File Explorer
Files and directories can be viewed in List View and Flow View mode:

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/3722198a-8cae-4837-95f2-e982b77e7f63" width=45% />  
  &nbsp; &nbsp; &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/5758b20e-22d1-4649-a683-17ff730e56aa" width=45% />  
</p>
