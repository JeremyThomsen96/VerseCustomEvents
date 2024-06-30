# VerseCustomEvents
CustomEvents_Verse_6_30_24


A Scuffed parametric implementation of subscribable events and an example of how you can do it per type if you're willing to type them out. 

Per type is more on par in terms of functionality at the moment, my brain isn't big enough to combat the no mutable members in paramteric classes yet. 

for the parametric implmentation you need to have your events as variables and manage them individually 

var MyEvent : generic_event(any_type) = generic_event(any_type){}

#Subscribing
set MyEvent = MyEvent.Subscribe(Some_Method_Here)

#Canceling
set MyEvent = MyEvent.Cancel()

The "Per Type" implementation can be used how epics events are used and since they inherit from all of epic interfaces they can be managed the same as epics events
