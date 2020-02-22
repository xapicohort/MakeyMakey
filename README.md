# MakeyMakey
Repo for MakeyMakey projects, this branch is for the Stage 1 Makey Makey app. This project is an output of the xAPI Cohort Spring 2020 hosed by TorranceLearning.

The goal of the stage 1 app is to build a LiveCode Community project, using LiveCode Open Source from https://livecode.org/.

The app can be clickon on via mouse, or with a connected Makey Makey board, used to test the connection of the Makey Makey board and to troubleshoot issues between the board and computer.

KNOWN ISSUE:
One of the default 'keys' the Makey Makey uses is a 'click.' When sending this signal by a connected Makey Makey the functions work as expected. However, during direct interaction with a mouse, any click sent to the arrow buttons or space button will ALSO register as a click, so that interaction is triggered as well.

OPERATION:
Each of the standard connections for the classic Makey Makey board (as opposed to Makey Makey GO) is mapped as keyboard input and detected via a series of IF statements. LiveCode recognizes the space bar and MouseUp (click) as distinct actions and sends messages to match: 'theKey is space' or MouseUp.

The arrow keys are handled differently, any arrowKey triggers an arrowKey message with a parameter stored as theArrow. The code tests via a if, else if, and else logical group to determine which arrowkey was pressed: Up,  Down, Left or Right. Once the if statements are complete, there is an else to pass the arrowKey, for other code to execute (if needed) and after the if there are statements that trigger no matter which arrow was pressed.

Reguardless of which interaction is used, the basic premise is that an interaction will:
1) Cause a beep sound, the mouseUp beeps twice -- audio feedback is provided
2) Set the hilite of the related button to true -- visual feedback is provided
3) We will wait 1/2 second for the visual feedback, then continue
4) ALL hilited objects are reset.

The logic structure and operation is currently coded in 46 lines of code, stored in the card object of the application. This is visble by downloading the LiveCode Open Source edition available free at LiveCode.org

As this application is available as a standalone file complied for Macintosh, Windows or Linux, it can be used offline as a testbed remote from internet access. Additionally, testing with this app allows the Makey Makey user to be assured that the board is working, without concern that the web page is having network, loading issues or internet connectivity problems.

This app will be published as Mac / Windows / Linux applications for the purpose of setup and troubleshooting the Makey Makey board, the project will also serve as the baseline for future projects for sending xAPI with Makey Makey. https://MakeyMakey.com



