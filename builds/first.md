# KBD75v2
My first attempt at building a keyboard will be with the [KBDFans 75v2](https://kbdfans.com/products/kbd75v2-custom-keyboard-diy-kit).  I wasn't sure about parting ways with the F-row (I use IntelliJ often) so I decided to go with the 75% profile.

## Bill of Materials

Components acquired for this build:

 - [KBDFans 75v2](https://kbdfans.com/products/kbd75v2-custom-keyboard-diy-kit) Kit with PCB, plate, case, stabilizers, and case foam.
 - [Cherry MX Silent Red Switches](https://kbdfans.com/products/cherry-mx-silent-red) I'm used to clacky reds and blues and wanted to try a silent variety.
 - [SA Retro Graffiti Caps](https://kbdfans.com/products/domikey-doubleshot-abs-sa-retro-graffiti-full-set-keycaps) I wanted to try the SA profile as they remind me of the caps I had on some of my first PCs.

Other components already on hand:

  - Soldering Iron (I think mine is X-Tronic Model #3020)
  - Solder Sucker
  - Kester Solder (I had SN63 PB37 @ 0.031")
  - Silicone Soldering Mat
  - Tweezers, Scissors, Side-Cutters
  - Teflon Grease
  - Glasses (for safety and readers)
  - Coffee (Counter Culture Forty-Six)

## Taking Inventory
Starting with the PCB and plate.  I needed to get my bearings.  Which way is face-up and North/South on this.

![PCB and Plate](./media/first/parts.jpg)

Something that I noticed on the board is that there was a small cluster of spare parts (resistors and diodes).  Not sure if this is common but I appreciated it.

![Spare SMT Parts](./media/first/spares.jpg)

A closer look at the bottom side of the board shows us the microcontroller being used.  We can see the [ATMEGA-32u4](https://www.microchip.com/wwwproducts/en/ATmega32u4) there with a 16Mhz crystal above and reset switch below.  I also just noticed the points for [ISP](https://en.wikipedia.org/wiki/In-system_programming).  You can also see the RBG LEDs for under-lighting.

![Microcontroller](/media/first/microcontroller.jpg)

## First Assembly (and first mistakes)
I noticed that most of the PCB suppliers recommend that before you do any assembly that you test each switch location.  Plugging the keyboard in and using a pair of tweezers to momentarily connect the two points for each key which monitoring the activated keys with a [keyboard testing application](https://www.keyboardtester.com/) showed that everything was OK.

Next I started by trying to figure out what to do first.  Do you put switches on the PCB and then the plate on top and where do these stabilizers go?  I reviewed the information on this [Techspot article](https://www.techspot.com/guides/1629-diy-build-your-own-mechanical-keyboard-part-2/) and determined that I should start with the stabilizers.

For my build I have what I think are Cherry Style Stabilizers (clip in).  I referenced this [Switch and Click article](https://switchandclick.com/stabilizer-guide/) on how to identify and improve stabilizers (band-aids, clipping, and lube).

Here I took a stabilizer apart and discovered that the clipping modifications were not necessary/possible.  (I'm not sure if this is due to a misidentification on my part or what).  I did go ahead and cut up a band-aid and apply below the backspace and space bar only.  Next a liberal amount of lube was added to the plastic on plastic bearing surface as well as where the metal bar clips on.

![Stabilizers](/media/first/stabs2.jpg)

With the stabilizers attached I then took a look at the switches that I am using.  I recall reading that there are a [few options](https://www.cherrymx.de/en/dev.html) for the switches.  There is a switch with and without mounting pins.  In looking at what I have I determined that I had the variety that you mount in a keyboard housing - the metal plate.

![Switches](/media/first/switches.jpg)

I placed a few of the switches into the plate, making sure to orient them in a direction that the contact pins are aligned with the through holes in the PCB.  I also spaced these first few keys closer to the edges to help in overall alignment of the plate and PCB.  I wasn't sure how much play there is this setup and didn't want to start working from one side going to the other and a find that small errors added up to the point where the last few columns would align well.

![First few switches](/media/first/first_switches.jpg)

At this point I began to solder the key contact pins to the underside of the PCB.  Plenty of space to work with and get the iron tip in and apply solder.  So no real problems here.  Started to move along at a steady pace.

I then noticed a mistake.  I had put a stabilizer across the area for the Right-Shift key thinking that this was required.  When I referenced a sample image of a completed build I noticed that I needed to squeeze in an Up and End key to the right of the Right-Shift.  With the stabilizer sitting in that spot I couldn't fit the Up key in.  In order to get that stabilizer out it seems that I would need to remove the plate - as the stabilizers are installed on the PCB first and then the plate with keys on top of that (sandwiching the stabilizer between the PCB and plate).  The keys that were already soldered down needed to be desoldered so that the plate could be lifted and the stabilizer removed.

With the mistake corrected I went about placing more switches and soldered them in place.  (Notice the nice little pile of solder removed by the desoldering sucker - this thing works very well.)

![More Switches](/media/first/more_switches.jpg)

Here we are with all the switches in place and plugged in and checking each of the keys with the [keyboard testing application](https://www.keyboardtester.com/) again.  All joints are good. 

![All Switches](/media/first/all_switches.jpg)

Next I set the assembled PCB into the case with the foam pad underneath.  The most challenging part of this was locating a small Phillips style screw driver that has a small diameter shaft to get to a couple of the screws that are in a deep counterbored hole on the bottom of the case.  Here is the PCB set in place with a few keycaps set on.

![Qwerty](./media/first/qwerty.jpg)

![Qwerty](./media/first/qwerty-2.jpg)

Here is the first take of all the keycaps set in place.  I am really liking the profile of these caps and the feel of the Red Silent switches.

![All caps on](/media/first/near_final.jpg)

I made a couple of small changes to the caps and layout to bring back a Delete key in the upper right corner (I feel like this might be necessary for some software).

![Final caps on](/media/first/final_layout.jpg)

## TODOs
 - Take a side profile pic to show the SA profile.
 - Show the Via setup.
 - Record the sound.  It is really very quiet and smooth compared to the Blue and Reds I've used in the past.