## Gesture-Recognition-Control-Powerpoint-Presentation

<img width="400" alt="Screenshot 2024-09-09 at 20 36 26" src="https://github.com/user-attachments/assets/a7ccf8be-49a6-4c42-88bd-6d05e0035546"> <img width="418" alt="Screenshot 2024-09-09 at 20 46 36" src="https://github.com/user-attachments/assets/21a60c47-d1be-442c-afc8-497243e8e2bd">

Gesture Recognition is an R&D project to control Microsoft Powerpoint while presenting on a large screen, using the Microsoft Kinect Sensor, C# and Kinect SDK. Using their right or left hand, the presenter can slide to the next or previous page. They can also zoom in or out by fisting their hand, and they can play or pause the presentation by displaying all or none of their fingers.

This project displays how to use the Kinect SDK to do basic gesture recognition to control PowerPoint.

## Requirements

-	Kinect for Windows SDK v1.7

Optional:

-	Microsoft Office PowerPoint 

## History:

v1.2 Updated for Kinect SDK v1.7. 

v1.1 Now updated for Kinect SDK v1.0. Speech recognition is on by default.

v1.0 Initial version.

## Usage

1.	Compile and run the application 

2.	Point the Kinect at you and stand at least five feet away 

3.	You can see yourself in the application window and the three circles will track your head and hands. 

4.	Extend your right arm to activate the "right" or "forward" gesture. Extend your left arm to active the "left" or "back" gesture. These gestures will send a right or left arrow key to the foreground application, respectively. 

5.	Run your PowerPoint show so PowerPoint is the foreground application, and the right and left gestures will go forward and back in your deck.

The ellipses grow and change color when your hand exceeds the threshold of 45 centimeters. The gestures will only activate once as your hand exceeds the threshold, and only one of the gestures can be active at once. You must bring your hand back closer to your body to activate the gesture a second time.

The gestures will also work for any other application. For example, open Notepad and type some text then use the gestures to move the cursor left or right one character at a time.

## Speech recognition

The speech recognizer is set up to recognize and respond to the following commands: 

-	computer show window 

-	computer hide window 

-	computer show circles 

-	computer hide circles

There is a four second delay after starting the program before the speech recognizer will respond.

## Limitations
1.	There is currently no way to activate embedded videos, so you should add a PowerPoint animation so the video starts when you push the right arrow key.

2.	The gesture is triggered based upon the distance between the head and the hands, so you might accidentally trigger the gesture if you put your arms out, or bend over to pick something up perhaps. 

