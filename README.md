# DTCAP (DJ twin deck console audio player.) 1.0

## What is DTCAP?
MPV is currently one of the best media player for linux. As it is mainly controlled by a console there is no inherently user interface.
DTCAP is actually a large bash script to offer a text user interface to simulate two audio (DJ) decks with MPV. So far DTCAP works on every linux system that offers a bash shell and runs the mpv media player.

## How do I run DTCAP?
If you have a linux system with a running bash ... install the MPV media player (i.e. with 'apt-get install mpv'). Then copy DTCAP to a place of your executeable path (i.e. /usr/local/bin) and start DTCAP in a console with 'dtcap'.
If you want to operate with high readability in a minimal sized window try something like 'xterm -fn terminus-32 -geometry 59x12 -bg black -fg white -e dtcap'.

## Are there any screenshots of DTCAP?

![dtcap](https://cloud.githubusercontent.com/assets/16148023/25332135/bc49337a-28e5-11e7-8fa4-fd3b4c96e1c0.jpg)

## Which features has DTCAP?
* Two music decks loadable from a file browser.
* Every deck is capable of play, stop, pause, volume control, forward, rewind and looping.
* An audio master with fader (left/right) and volume control.
* 

## How do I set the default music library?
To set the audio directory DTCAP starts with ... edit DTCAP and search for the line that starts with '# audio_dir="/"', uncomment it and expand "/" to the path of your music library.



## How do I set the equalizer?
Setting the equalizer is not yet implemented. So far you can edit DTCAP, search for the eqaulizer section and set and name a profile for the 10-band-equalizer. Then assign this profile to deck A and/or deck B. See the existing examples in DTCAP.

