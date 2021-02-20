# Logic Pro template for Spitfire Abbey Road One: Orchestral Foundations V1.0.0 (2021-01-23)

Copyright (c) 2021 by Justin L. Franks (justin.franks@gmail.com). Licensed under the GPL V3 license.

___Feb 20,2021 NOTE:__ This template and the patches it uses were created with version 1.0.2 of the Abbey Road One library. It needs some minor updates to be fully compatible with the current version of the library (v1.0.7). This should be done in the next few days._

## Overview ##

This is a Logic Pro template for Spitfire Audio's Abbey Road One: Orchestral Foundations sample library. It is similar to the template provided by Spitfire for their BBCSO libraries.

___IMPORTANT:__ All of the instances of the AR1 plugin in this template are loading a user preset which only includes the specific articulations which are used. Each of these presets are included with the template. You just need to copy the 'user' folder into the 'Templates' folder of your copy of AR1. If you have created some of your own presets before, then the 'Templates/user' folder already exists in your copy of AR1, so just copy the contents of the 'user' folder into the 'Templates/user' folder._

Each category of instruments (Full orchestra, Strings, Brass, Woodwinds, and Percussion) has its own track stack, with three busses for different types of articulation:

__Full orchestra:__ Longs, shorts, swells 

__Strings:__ Longs, shorts, pizzicato + tremolo

__Brass:__ Longs, shorts, swells

__Woods:__ Longs, shorts, swells

__Percussion:__ Drums, metals, tuned

Each section available in the library (high strings, horns, low woods, etc.) has three tracks, corresponding to each of those busses. Percussion has individual tracks for each instrument (bass drum, suspended cymbals, glockenspiel, etc.).

Only the default Mix 1 mic is used for all instrument tracks.

There is also a reverb send for each track stack. I use R4 for reverb, but changed this to the Chroma reverb included with Logic for compatibility. All of the reverb sends are turned on, with just a touch of reverb added. Long articulations have the highest amount of reverb, followed by swells, with short articulations having the least reverb.

Each track also has a Gain plugin added for balancing. I only did a very quick and rough balancing, to the neighborhood of -12 dB (and peaking up to around -6 dB depending on the instrument) for three or four simultaneous notes played at maximum dynamics / velocity. This *will* need adjustment to your own preferences, but should give a decent starting point.

### Routing ###

__Section articulation type(s) ==> Full section articulation type(s) ==> Full section ==> Full mix__

So, for the low string longs, it is _Low strings longs ==> Strings longs ==> Strings ==> Full mix._

### Bussing ###

#### Instrument Stacks ####
__Bus 10:__ Full orchestra

__Bus 20:__ Strings

__Bus 30:__ Brass

__Bus 40:__ Woodwinds

__Bus 50:__ Percussion

__Bus 250:__ Full Mix

#### Instruments ####
__Busses X1-X4:__ Articulation type(s).

__Bus X1:__ Longs (for Percussion: Drums)
    
__Bus X2:__ Shorts (for Percussion: Metals)
    
__Bus X3:__ Swells (for Strings: Pizzicato & Tremolo, and for Percussion: Tuned)
    
__Bus X4:__ unused

_(Bus 11 for Full Orchestra Longs, Bus 42 for Woods Shorts, Bus 53 for Tuned Percussion, etc.)_

#### Submixes and Effects ####
__Busses X5-X9:__ Effects sends

__Bus X5:__ Reverb

__Busses X6-X9:__ unused

_(Bus 25 for Strings Reverb, Bus 35 for Brass Reverb, and so forth. You can use the X6-X9 busses for any additional effects sends for each track stack.)_
