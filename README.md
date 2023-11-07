# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:
Visual Components Premium 4.3

## Procedure:
1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
pos = [[1,30],[2,40],[3,90]]
robot = getRobot()
robot.driveJoints (0,0,0,0,0,0)
delay(5)
for i in pos:
robot.Controller.moveJoint (i[0],i[1])
delay (5)

```
## Output
### 1. Generic Articulated Robot
![280909520-d8ffe31e-a088-42b1-a026-87eb1d14a801](https://github.com/Darkwebnew/Movement-of-Robot-Joints/assets/143114486/1c5832be-dfd0-4dd4-9444-96c5e01e23f8)
### 2. robot.driveJoints(0,0,0,0,0,0)
![280909488-8b804be2-03cd-432d-99f3-d953001ca00e](https://github.com/Darkwebnew/Movement-of-Robot-Joints/assets/143114486/ef2a6e30-f87c-4df2-935e-9cfb5b06a107)
### 3. Movement of Joint1
![280909438-573a3295-f5c0-4373-90ce-03e1bcf2b798](https://github.com/Darkwebnew/Movement-of-Robot-Joints/assets/143114486/3177fa26-2033-48e4-a8eb-7ead9c711e9d)
### 3. Movement of Joint2
![280909384-3838686b-cc2e-4460-9757-75d6f2d5c366](https://github.com/Darkwebnew/Movement-of-Robot-Joints/assets/143114486/5a629638-c63e-4faf-9928-8a6461d6aea3)
### 3. Movement of Joint3
![280909325-af92e9ca-b3bb-4f46-8a0a-7e5207b0e76f](https://github.com/Darkwebnew/Movement-of-Robot-Joints/assets/143114486/4c9f7213-a9c8-4d2f-bfd7-54dbf04763d2)
## Result 
Thus the different robots joints are moved with the help of python list.
