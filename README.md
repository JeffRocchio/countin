## Purpose

This repository contains assets for making, and improving, a musical count-in soundfont. Please refer to Musescore forum topic [count 1+2+3+4+](https://musescore.org/en/node/51031).

I am here just sharing out what I did for my own use. Maybe folks will contribute and we can collectively make something better than what I did.

## Disclaimer 

Please note that I didn't attempt to make it very high quality because I just wanted to see if the idea would work. But what I ended up creating has proven good enough that I haven't yet bothered to go back and improve it. 

## How I Made the Counting Soundfont 

   1. I figured I needed to pick a max tempo to count at. Given that I, and my little neighboorhood group, are beginner/intermediates I decided that for our purposes we could top out at 140 BPM.
   
   2. I set my metronome to 140 BPM, put on my headphones to listen to it, and counted into a microphone to the metronome beat. I counted a dozen or 'streams' of numbers - "1 2 3 4 5 6," pause, "1 2 3 4 5 6," and so on. Then I did that again trying to make emphasis counts for the downbeats. I also did "One Measure," "Then," and "On." This enables me to have the countin in instructions to kick off with - as in "One measure, then on 3."
   
   3. In my case I'm a Linux guy, and I use Ardour as my DAW. So I brought my audio file into Ardour and spent probably 2 hours or so picking the best sound samples for the counts and editing them for the proper start and endpoints. I didn't even try to normalize levels, which will be obvious if you try my sound font.
   
   4. I wrote down a 'map' for each counting sound sample and the notes to assign them to - in my case using the key of D. Key of D because I am a mountain Dulcimer player, so 90% of all my tunes are in that key, thus it's convenient to use that for my counting. So, for example, D4 is the sound "One," E4 is "Two," F#4 is "Three," etc.

   5. I distinguish between normal beats and emphasis beats by using the midi volume parameter. If you set the note's volume above 86 you get the emphasis sample, below that you get the normal sample.

   6. As one should always do when making a soundfont, I named each of my little sound samples with a consistent naming convention and brought them into Polyfone to make the sound font.

   7. Then, of course, on Linux to use the sound font in musescore I simply copy the sound font to the user/share/soundfonts directory. Then Musescore just sees it. When I want to use it I create an instrument I call "count," select my 'CountIn' soundfont in the mixer, and away I go.
   
   8. What I do is add a few measures to the beginning of the song. My habit is to leave the 1st measure empty to have one measure of silence to begin. Then I have a measure which gives the instructions - e.g., "One measure, then on 3." Then I have the countin measure. I set the 'Actual' number of beats in this measure to match the total countin. So, for example, in a 4/4 tune that begins with 3 pickup beats I'll set the measure to 7 actual beats so that I have a countin that goes: "1 2 3 4 1 2 3."
   
   9. I also generally produce audio files with 3 verses for practice purposes. So, as needed, I'll add repeats in the appropriate places so that the playback does that. (Often making use of the 'Play count' property on a measure with an ending repeat.)

## Assets and Examples

Example_Old-Irish-Blessing_120bpm.mp3 - example of an actual audio file using my counting soundfont.

Example_Old-Irish-Blessing_4midi.mscz - The Musescore score used to create the example mp3.

CountIn_v01.sf2 - My counting soundfont

count-note-map.txt - Shows which notes to put on the staff to get which counting sounds.
