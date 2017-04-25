# DTCAP (DJ twin deck console audio player.) 1.0

## What is DTCAP?
MPV is currently one of the best media players for linux. As it is mainly controlled by a console there is no inherent (graphical) user interface. DTCAP is actually a large bash script to offer a simple, fast and powerful text user interface to simulate two audio (DJ) decks with MPV. So far DTCAP works on every linux system that offers a bash shell and runs the mpv media player.

## How do I run DTCAP?
If you have a linux system with a running bash ... install the MPV media player (i.e. with 'apt-get install mpv'). Then copy DTCAP to a place of your executeable path (i.e. /usr/local/bin) and start DTCAP in a console with 'dtcap'. If you want to operate with high readability in a minimal sized window try something like 'xterm -fn terminus-32 -geometry 59x12 -bg black -fg white -e dtcap'.

## Are there any screenshots of DTCAP?

![dtcap](https://cloud.githubusercontent.com/assets/16148023/25332135/bc49337a-28e5-11e7-8fa4-fd3b4c96e1c0.jpg)

## Which features has DTCAP?
* Two music decks loadable from an inbuilt file browser.
* Every deck is capable of play (progress), stop, pause, volume control, forward, rewind and looping.
* An audio master with fader (left/right) and volume control.
* AutoDJ: Plays files of a directory random on deck A.
* Dynamic CPU load control - reduces CPU load gradually if not needed.

## With which keys can I control DTCAP?
In principle you are free to edit DTCAP and assign your own key to the appropriate case-statement. The default assignment works with four cursor key areas:
* Q W E A S D: Control deck A (pause, vol+, play/stop, fwd, vol-, rew)
* R T Y F G H: Control the master (play_A, vol+, play_B, fade_left, vol-, fade_right)
* U I O J K L: Control deck B (pause, vol+, play/stop, fwd, vol-, rew)
* SPACE UP ENTER LEFT DOWN RIGHT: File browser (load_A, up, load_B, page_up, down, page_down)

And some other keys:
* / - <: One directory up
* TAB BACKSPACE: Refresh display (sometimes needed)
* 5 6: Set loop for deck A or B
* P 0 3: AutoDJ on deck A
* X ESC: Exit
* ?: Help

## How do I set the default music library?
To set the default audio directory, edit DTCAP and search for the line that starts with '# audio_dir="/"', uncomment it and expand "/" to the path of your music library.

## How do I set the equalizer?
Setting the equalizer while running is not yet implemented. So far you can edit DTCAP, search for the equalizer section and set and name a profile for the 10-band-equalizer. Then assign this profile to deck A and/or deck B. See the existing examples in DTCAP.
