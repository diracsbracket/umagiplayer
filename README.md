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
* Audio control: Balance, Volume, Equalizer
* Analyzer: Bar, Block, Boom, Turbine

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
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/5758b20e-22d1-4649-a683-17ff730e56aa" width=45% />  
</p>

<img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/d851669f-319f-4752-a47d-247bcac205dc" width=45% />

## Playlists
<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/c5a291af-dee3-4a86-a692-59789a253685" width=45% />
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/2e0649a0-50eb-43f1-87ae-992c21c41579" width=45% />    
</p>

There is also a dedicated playlist for Internet Radio channels:
<img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/0834d19a-c127-4ad3-b7cc-99fa277931cf" width=45% />
