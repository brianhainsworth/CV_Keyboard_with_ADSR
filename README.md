# CV Keyboard with ADSR
A CV/GATE keyboard with ADSR for Eurorack or other modular synthesizers 

So I had been hanging out for a really simple little CV/GATE Keyboard for my modular setup. Like I've got a Beatstep, but having to get that out and separate power.... ugh. Instead I wanted something smack bang right in the rack, Easy peasy! I couldnt find anything that was in a Euro format so thats why I have put this together.

## The Design / Stealing from more talented people

Sure I think something could be done with arduino really easily, but the amount of times I've just been confused with the coding lead me to to [Ken Stones CGS-10](https://www.elby-designs.com/webtek/cgs/cgs10/cgs10_pedal.html). Ken Stone's design was for a matrix style keyboard which could be hooked up to an existing keyboard or buttons wired. His design is a little more than 1 octave, but because of size limitations and wanting it to look a bit pretty, I chopped off a couple notes. I have left the X and Y points for the matrix so if you wanted you could ignore the keyboard on the PCB and wire up your own buttons.

The keyboard uses a *Keyboard scanning chip, a 74C922* these seem to be a bit tricky to find these days, but I found one on [eBay.com](http://www.eBay.com), heck, they are probably knock-offs, fakes, whatever, but they do the trick. I wont link to them though as the listing will probably expire but just search geez. The 74C922 is the only kinda weird thing in this build, the rest came from [Tayda](https://www.taydaelectronics.com/) no worries.

I went for a 100mmx100mm PCB so I could get it in one of those cheapy deals from a PCB manufactuererer, it gives me enough space for the keyboard along the bottom without doing some weird horizontal thing. 
After putting the keyboard side of things together, I realised that there would be a bunch of space left over. I thought maybe a clock, but whatever a clock doesnt really relate to a keyboard, so I went with an ADSR.

The ADSR is taken from [Benjie Jiao's MiniADSR](https://benjiaomodular.com/post/2022-02-02-mini-adsr/) which in turn is taken from [René Schmitz' Fastest Envelope in the West.](https://www.schmitzbits.de/adsr.html) I like Benjie, he has always been kind, replies to me on insty and makes some cool stuff. 

I slapped the ADSR together and hooked the gate out from the keyboard straight to the ADSR so that way if you dont have anything plugged into either of them the gate will trigger the ADSR so it all works together. BUT you can still use them independently from each other etc etc blah blah blah

Also the schematic here is a mess, I'm not going to tidy it up, sorry not sorry.

## Panel stuff

I make my panels out of 3mm acrylic / perspex. I get them laser cut at a local(ish) place which costs hardly anything. Your local library or makerspace could also do this for you. I suppose I do this as I reckon they would look terrible if I cut them myself out of aluminium or whatever. I suppose I could get them done at a metal fabricators. 

ANYWAY 3mm acrylic is sturdy enough (2mm is not), I can paint it afterwards if I want and I can leave the LEDs under, not poking through. I think this will become more handy as Im starting to get brave enough to do some SMD stuff. I'm getting off track here...

With the 3mm acrylic there are a couple considerations...
- You gotta counter sink (not sure if that the right term) the PJ-3001f jacks. They have a little bit of a edge that makes things not sit flush. Use a stepped drill bit or you might shatter the acrylic.
- You gotta use the cheaper not threaded potentiometers. The height clearance of these means that the keyboard section will be too low on the panel, but maybe your into that, whatever. If I had picked different buttons you could probably use the threaded pots.


## Credits ###

CV/GATE keyboard design by Ken Stone - copyright 2001 by Ken Stone

MiniADSR design by BenjiaoModular - Copyright (c) 2022 Benjamin Joseph Jiao. Used under MIT License
