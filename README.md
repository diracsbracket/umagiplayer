# umagiplayer
QML frontend to Clementine Music Player for Raspberry Pi with touchscreen

# Objective
Create a dedicated, standalone and connected music player based on Clementine and Raspberry Pi.

The aim is to house a Raspberry Pi 4 with touchscreen, SSD drive and rotary encoder
control knob into a HiFi component form factor, maybe as follows:

<img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/8a3429f1-4257-4a73-ad7d-acc8a125e579" width=65% />

The desktop Clementine UI is replaced by a QML-based version suitable for an embedded system with a small 800 x 480 touchscreen.

My development setup looks currently as follows:

<img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/ef6fd268-2674-4d6b-b3f2-bc894988a204" width=92% />

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/0faccf82-df43-454a-a3df-67406ffd9e6b" width=45% />  
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/eeae22cc-b22e-4f61-9d46-a19cd0c1b04c" width=45% />  
</p>

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/1fc90bda-aea8-4c38-9781-266f797fe224" width=45% />  
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/0d2b83b3-d1f0-4198-b6f2-594c4aeec173" width=45% />    
</p>

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

Art embedded in the audio files is also shown:

<img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/d851669f-319f-4752-a47d-247bcac205dc" width=45% />

## Library

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/0f12ec50-af5c-4e84-b7c8-e9f97be90479" width=45% />  
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/69ad53e0-f62b-41c1-86ae-9cd8b13a5f7f" width=45% />  
</p>

## Playlists
Playlists can be created by selecting files or folders in File Explorer or by selecting songs and albums from the Library.

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/c5a291af-dee3-4a86-a692-59789a253685" width=45% />
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/2e0649a0-50eb-43f1-87ae-992c21c41579" width=45% />    
</p>

There is also a dedicated playlist for Internet Radio channels:

<img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/0834d19a-c127-4ad3-b7cc-99fa277931cf" width=45% />

## Internet Radio
Of the online radio streaming services accessible in Clementine, only Icecast and Radio-Browser.info are currently implemented.

<ins>Icecast:</ins>

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/3b6ea6e6-5514-4ef6-9daf-5008d69fa25d" width=45% />
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/42aebaf6-3b6a-442e-a16c-4cd90ac3ebf8" width=45% />    
</p>

<ins>Radio-Browser.info:</ins>

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/76899cb6-fa60-4e02-bbe5-c549041c862d" width=45% />
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/124b3221-8ce6-42b6-8403-9cf126eb142d" width=45% />    
</p>

Unlike Clementine, selected radio channels are not added to the current playlist but to the dedicated Internet Radio playlist.
