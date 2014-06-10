magtimer
========

A one-page HTML+JS concert countdown clock for stage managers to display time and songs remaining to bands on-stage

Working demo here: http://magfest.org/demos/magtimer/magtimer.html

Design goals:
- Only one HTML page, no external dependencies not embedded in the page
- Works completely offline in any HTML5 browser or phone
- Should be visible to the band playing so they can see how much time is remaining and whether they are OK to play another song

This is a countdown timer for use by stage managers in helping manage bands to make sure they stay on-time.

Timers
===
There are two timers you can set:
- Setup time (amount of time a band has to setup and soundcheck)
- Playing time (amount of time a band actuall plays)

For example, you might give a band 20 minutes to setup, and 40 minutes to play.

The timers will output 

Timer 1 - The Setup Timer
===========
When you start the setup countdown, the display will read SETUP.  
If a band finishes their setup early, click 'Skip Setup' and it will jump to the Playing timer

If the setup timer goes to zero, it will automatically begin the Playing Timer.  
This indicates you are behind schedule, and now the band is eating into the playing time.

Timer 2 - Playing Timer
====
This timer will be:
GREEN if a band is OK to play one more song (time > 5mins)
YELLOW if a band should only play one more song (time < 5mins)
RED if a band should not start another song after this one (time < 2mins)
FLASHING LIKE CRAZY AND FLIPPING OUT if they're out of time.
