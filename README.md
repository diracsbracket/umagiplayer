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
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/071e99dd-3072-43fd-b0a8-be9286a9346a" width=45% />
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
This section contains a few screenshots made directly from the Pi4, showing the QML interface.

## Main screen

<img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/b6ae0049-8f0b-4c19-9215-aaec6b1c20e6" width=45% />

## File Explorer
Files and directories can be viewed in List View and Flow View mode:

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/3722198a-8cae-4837-95f2-e982b77e7f63" width=45% />  
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/5758b20e-22d1-4649-a683-17ff730e56aa" width=45% />  
</p>

Navigation and selection through the File, Library and Playlist views can be done using the touchscreen or via the rotary encoder. 

Art embedded in the audio files is also shown:

<img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/d851669f-319f-4752-a47d-247bcac205dc" width=45% />

## Library

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/0f12ec50-af5c-4e84-b7c8-e9f97be90479" width=45% />  
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/69ad53e0-f62b-41c1-86ae-9cd8b13a5f7f" width=45% />  
</p>

## Internet Radio
Of the online radio streaming services accessible in Clementine, only Icecast and Radio-Browser.info are currently implemented.

### Icecast

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/3b6ea6e6-5514-4ef6-9daf-5008d69fa25d" width=45% />
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/42aebaf6-3b6a-442e-a16c-4cd90ac3ebf8" width=45% />    
</p>

### Radio-Browser.info

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/76899cb6-fa60-4e02-bbe5-c549041c862d" width=45% />
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/124b3221-8ce6-42b6-8403-9cf126eb142d" width=45% />    
</p>

Unlike Clementine, selected radio channels are not added to the current playlist but to the dedicated [Internet Radio playlist](#internet-radio-playlist).

## Playlists
### Album playlist
Playlists can be created by selecting files or folders in File Explorer or by selecting songs and albums from the Library.

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/c5a291af-dee3-4a86-a692-59789a253685" width=45% />
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/2e0649a0-50eb-43f1-87ae-992c21c41579" width=45% />    
</p>

### Internet Radio playlist
There is also a dedicated playlist for Internet Radio channels:

<img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/0834d19a-c127-4ad3-b7cc-99fa277931cf" width=45% />

## Analyzer

### Volume and Balance

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/9f68f886-43f3-4b9b-bf7c-bfd0fb1975c2" width=45% />
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/e60c0fbb-cc11-4d28-800c-35f6832d1553" width=45% />    
</p>

### Equalizer and Compressor
A QML interface to the Gstreamer equalizer plugin used by Clementine is provided, and an audio (dynamic range) compressor was added.

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/6233884c-e16c-4275-b7df-90bb4ca4ac9c" width=45% />
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/3e7b5515-bfb6-46e8-b526-395102b71775" width=45% />    
</p>

### Audio Analyzer
The Bar, Block, Boom and Turbine analyzers from Clementine have been reused in simplified form and a VU meter was added.

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/a0e42e9c-420e-4b72-a878-08588a621a54" width=45% />
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/f3f16c81-86dc-4fba-ae8b-faf6daa886d4" width=45% />    
</p>

### Settings
Currently only a limited subset of the Clementine settings is provided:

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/acafb3d3-c728-4dfc-a98d-7d0cd9ed5aa0" width=45% />   
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/249eb1ac-7169-4d74-b171-171af72f3a26" width=45% />
</p>

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/1cccfb34-be7b-46b5-a78c-be589b9233ec" width=45% />   
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/cea325a6-ef5e-403a-80f0-8b1efde117aa" width=45% />
</p>

### Performance Monitor
A simple performance monitor for CPU, memory, network and disk and process usage was added for fun.

The network monitor can be used for instance to get the IP address of the Pi device, in case you wish to SSH into it.

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/bedb9891-0bc0-452e-81f7-08713e7b7088" width=45% />
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/9f841394-3b7d-456f-a332-2a60536e30aa" width=45% />
</p>

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/d88272a2-25b7-4f76-8aa7-e21ecef286dd" width=45% />
  &nbsp; &nbsp;
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/c459e0a1-a560-4596-a5f0-4f458f72dfe5" width=45% />    
</p>

<p float = "left">
  <img src="https://github.com/diracsbracket/umagiplayer/assets/13051119/cb0264cf-95e7-42e6-9868-e05b95335a12" width=45% />
  &nbsp; &nbsp;
</p>

