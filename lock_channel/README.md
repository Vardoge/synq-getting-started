Lockbot
=======
At SYNQ, we use our friendly neighborhood lockbot on #lock to keep track of our 
resources.

It can be used to lock and unlock resources, reminds uses what items are locked 
once every hour, and keeps track of who locked an item and when.
 
Below is a command list of all of commands supported by lockbot. 

**Lockbot commands**:
 * `lockbot	 help`/`lockbot commands` : this list
 * `list locks`/`what is locked`/`what's locked`: List items that are currently 
locked
 * `lock: [...]`: lock an item under your name
 * `unlock: [...]`: unlock an item you own
 * `force unlock: [...]`: unlock an item regardless of who owns it(use with 
caution)
for example, SANTA can send the message `lock: christmas` on #lock to signal that 
he will be locking the resource `christmas`

While it is locked, no one else can access this resource without permission from 
SANTA.

If anyone tries to message `lock: christmas`, lockbot will give an error, as it is 
already locked.

Additionally, SANTA will be reminded once every hour that he is hogging the 
resource.

This continues until SANTA messages `unlock: christmas`, or anyone calls `force 
unlock: christmas`, at which point `christmas` is freed.

Guidelines
==========

Below is a list of guidelines to follow when working with resources on #lock

 * When locking an item, use all-lowercase letters, and only use the following 
characters:
	* letters `a-z`
	* digits `0-9`
	* special characters `_ . = - < > : / | ( ) { } [ ]`
 * When locking a server, use full name, eg. `experimental.synq.fm` instead of 
`experimental`
 * When locking part of a resource, use forward slashes to divide levels, eg. 
`shrek.synq.fm/nginx` instead of `nginx on shrek.synq.fm`
 * When part of a resource is locked, the full resource can't also be unlocked, eg. 
can't have `shrek.synq.fm` and `shrek.synq.fm/nginx` locked at the same time (this 
is currently not handled by the bot) 
 * After 06:00 CET the day after an item is locked, other people are allowed to 
unlock it with `force unlock: [...]`, *unless otherwise is specified by the person 
who locked it*(this is currently not handled by the bot)


TODO/DESIRED FEATURES
=====================
 * handle sub-resources
 * add `force unlock:`-blocking timers
 * remember *lock:* collisions (and notify those who ask for a lock when unlocked)

