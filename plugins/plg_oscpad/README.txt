ABLETON LIVE PAD 
RELEASE 0.5

THIS IS AN EXPERIMENT ONLY!!!!!
it is not finished, and has a number of shortcomings its really just a demo to play with at this stage

Ive played with it on a demo of Live 9, but should work on 8 too


TO USE:
a) first install LIVE OSC , following instructions at
http://livecontrol.q3f.org/ableton-liveapi/liveosc/
b) In ableton, setup LiveOSC as control surface in preferences
c) Install plugin into EigenD. under /usr/pi/release-2.0.74-stable/plugins/Eigenlabs/   (or you can add to your path if you know how ;))
cd /usr/pi/release-2.0.74-stable/plugins/Eigenlabs/
tar xvf ~/Downloads/plg_oscpad.tar
d) start EigenD, and in workbench create a new 'osc pad' agent, and connect it to the keyboard (or probably a keygroup too, but not tried that ;))


press keys on your pico (etc) to record/launch clips.
green = playing
orange = availble not playing
red = recording
off = nothing there


properties:
top, left, width, height
e.g. 
osc pad hey set width to 8
osc pad hey top up

arrangment
e.g 
osc pad hey arrangement to 1 set ; starts playing scene 1
osc pad hey arrangement up ; move to scene 2
osc pad hey arrangement ; move  back to scene 1

verbs
reset - refresh, use when new are loading a new set in live, or restarting live
play - start playing
stop - stop playing
e.g
osc pad hey reset
osc pad hey play
osc pad hey stop



known issues :
main issues fixed in 0.2-0.4


change log
0.1 - initial release
0.2 - improved colours, and recording behaviour, fix toggle clip
0.3 - initial load state
0.4 - introduce moveable view port, fix mem leak, consistently call osc pad
0.5 - fix bug where it would launch clips outside of view
0.6 - reset to refresh, transport controls, added verbs play,stop and attribute arrangement = scene play



