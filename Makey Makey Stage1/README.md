# Stage 1: MakeyMakey Setup and Testing App
Our goal is to build a cross platform app for setup and testing of the Makey Makey
The initial build is desktop only (MakeyMakey is USB device): Mac/Win/Linux
Request team & other cohort members to test the desktop and provide feedback 
	 in the #Team-MakeyMakey slack channel

There is a video demo of the app on [YouTube](https://www.youtube.com/watch?v=DJedJ5IjPsw):https://www.youtube.com/watch?v=DJedJ5IjPsw

KNOWN ISSUE: One of the default 'keys' the Makey Makey uses is a 'click.'

When sending this signal by a connected Makey Makey the functions work as expected. 

However, during direct interaction with a mouse, any click sent to the arrow buttons or space button will ALSO register as a click, so that interaction is triggered as well.

## Setup and testing with MakeyMakey board:

### Setup the Makey Makey
1. Plug the board in via USB
2. Each of the lights should cycle on then off
3. The red power light on the back of the board remains lit

### Testing the MakeyMakey Software
1. Download the 'MakeyMakey' app from the [GitHub Page](https://github.com/xapicohort/MakeyMakey/tree/master/Makey%20Makey%20Stage1):
https://github.com/xapicohort/MakeyMakey/tree/master/Makey%20Makey%20Stage1
2. Launch the 'MakeyMakey' app (exe, app, or tz for linux?)
3. Click each of the buttons:
RESULTS The app should respond with each button hilting, a sound, then the button return to normal.
4. Connect the MakeyMakey board, use the alligator clips for each button and the Earth / Ground bar
5. Tap the ground lead to one of the buttons on the board, or to the connected lead
6. The Green light should light up on the MakeyMakey board, AND the button should flash, a beep be heard 
NOTE: This is the SAME result as #3 above.

If each of these steps is successful, the MakeyMakey board is operating correctly and ready for your project.

If you have no light flash, no button halite on the screen, o no click: 
* check your connections to the MakeyMakey board.
* check that the red light is lit on the back.
* check the USB cable is securely fastened to the computer, and the other end connected to the MakeyMakey board

