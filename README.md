https://artlee17.github.io/MidiControlledAudioPlayer/

I used Gemini to build a Midi Controlled Audio Player

MIDI CHART:
PLAY - CC 109 Value 127
PAUSE - CC 109 Value 0
PREVIOUS SONG - CC 110 Value 0
NEXT SONG - CC 110 Value 127

CC 108 Selects song in playlist. Value 1 would select song 1, value 2 for song 2, etc.

When selecting song via MIDI 108 or 110 song will not auto play. It will just load the song.
Then use CC 109 to play/pause. 

The button to the right of the next song button is an autoplay button. When engaged, when 
the current song ends the next song in the playlist will start playing. When the autoplay 
button is disengaged all playback stops as soon as a song ends. The default state is off.

I made this to jam along to backing tracks and to be able to control it all from my
midi foot controller. It works well but since it is web based it does not save the playlist
if the page is closed or refreshed. One workaround is to name all of your tracks with numbers at
the start (001 - Track 1, 002 - Track 2, etc.) and add them to a folder and then just select all
to add them all at once and they will stay in the correct order.

My goal was to make this into a VST/Plugin but I am not a coder. I got somewhat close using
Gemini, JUCE, and Visual Studio but still had a few errors I could not work out.
So if anyone wants to give that a shot that would be cool. Enjoy!

