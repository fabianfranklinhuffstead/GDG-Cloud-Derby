# GDG - Cloud derby (Hackathon)

<img width="50%" height="50%" src="/media/feature-1.png"/>

Task:

The reason for the cloud derby is to spend 8 hours to build a robot. To 
control a robot to play a comptetive soccer 'like' game set with four 
robots and four different corners. Different balls will have colors assigned. 
Robots will collect 3 balls and return them to its corner. It takes a picture
uploads to IOT core. Which stores in a node REST point and processes on Tensorflow.


There are several elements of the task itself however there are extras including
using diagflow for voice control. There will be portions of the project where
we will build cars and other portion which are base on adminstration using big query
to view data JSON responses.

Key points:
Edudcation should be fun

Architecture user flow diagram:
<img width="50%" height="50%" src="/media/architecture-1.png"/>

Architecture technology flow:
<img width="50%" height="50%" src="/media/architecture-2.png"/>

## Resources

Rules:
https://www.cloudderby.io/getting-started/game-rules

Credentials:
(ommited)

Work doc: https://docs.google.com/document/d/1PVv9Pstwpu9DWkVE05a4GN8UD90YD2sF53v1C8u6s3Q/edit#

High level initial setup:
1. Complete the initial Project Setup.
2. Deploy and start Object Detection Module on the cloud
3. Deploy and start Control Module on the cloud
4. Provision and start GoPiGo Car software on the car
5. Go to the Game Control web App and start the game, see URL in the log for the Cloud Control Module.

Project ID: robot-derby-fabian
Update file $HOME/setenv-dev-workspace.sh with the proper values for $ZONE and $REGION:
REGION = europe-west4
ZONE = europe-west4-a

Copy all images from gcloud to robot vm
command - gsutil -m cp -r gs://robot-derby-team27-images/* c:\a-robot-images

Example ball detection images:
<img width="50%" height="50%" src="/media/ball-detection.png"/>

## Hackathon material

- Overview
- Architecture
- Conventions
- Project creation and setup
- Machine learning image preparation
- ML Model Training
- Driving controller
- GoPiGo Car assembly and setup
- ML inference
- Voice control with control Google assistant and dialogueflow
- Troubleshooting
- Game preparation and play
- Optional: Calibrate car lens (was not optional)

https://www.couldderby.io

Important formulas include:
Object height on sensor (mm) / focal length (f, mm) = Real Object height (mm) / Distance to Object (d, mm)

Which calculates shift from the middle of the image knowing the angle of view of the lens

<img width="50%" height="50%" src="/media/camera-tracking-formula.png"/>

## Result

Pi Robot 1:

<img width="50%" height="50%" src="/media/pi-robot-1.JPG"/>

Pi Robot 2:

<img width="50%" height="50%" src="/media/pi-robot-2.JPG"/>

Track 1:

<img width="50%" height="50%" src="/media/track-1.JPG"/>

Track 2:

<img width="50%" height="50%" src="/media/track-3.JPG"/>

Recording results:

<img width="50%" height="50%" src="/media/track-2.JPG"/>

Video:

<object width="425" height="350">
  <param name="movie" value="/media/robot-track.MOV" />
  <param name="wmode" value="transparent" />
  <embed src="/media/robot-track.MOV"
         type="application/x-shockwave-flash"
         wmode="transparent" width="425" height="350" />
</object>

