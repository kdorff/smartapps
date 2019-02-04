# Re-Auto Lock Door

I've been a long time user of "Enhanced Auto Lock Door" by Arnaud 
[Original source code|https://github.com/SmartThingsCommunity/SmartThingsPublic/tree/master/smartapps/lock-auto-super-enhanced]
(found in the SmartThings SmartApp store). I believe the original author 
had a slightly different intent - a sensor that physically separated from 
the lock in question so the sensor can also unlock the lock. In my scenario,
there is never a case where I want the SmartApp to execute Unlock.

My goal was to have the sensor be on the door iteself and this SmartApp
is designed to keep that door locked. Simply put:
This software monitors the Open/Closed Sensor and Lock for events. If an event shows
the door is closed yet unlocked, it will wait N seconds and then lock the door.
If the door opens or you lock the door within the N seconds, the re-lock
will be cancelled (until the door closes).
