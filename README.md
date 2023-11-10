# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
  
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
  
3. 	In the script editor, add the code and then compile the code.

## Program:
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
## Outputs:
### 1. Generic Articulated Robot

![image](https://github.com/swethaselvarajm/Movement-of-Robot-Joints/assets/119525603/f08ac665-f1b7-426f-8a08-50a477f09ce2)

### 2. robot.driveJoints(0,0,0,0,0,0)

![image](https://github.com/swethaselvarajm/Movement-of-Robot-Joints/assets/119525603/cf2e8fdb-f46c-4196-8c92-b08afa54dcf7)

### 3. Movement of Joint1

![image](https://github.com/swethaselvarajm/Movement-of-Robot-Joints/assets/119525603/e1e2a049-4523-4af9-b51d-22fdb2dca56a)

### 4. Movement of Joint2

![image](https://github.com/swethaselvarajm/Movement-of-Robot-Joints/assets/119525603/0cb14a03-9e6f-4f01-800f-d6f490e53fe3)

### 5. Movement of Joint3

![image](https://github.com/swethaselvarajm/Movement-of-Robot-Joints/assets/119525603/d57c51fe-5f67-43c0-a8b6-c82f4dc8c1d7)

## Result :
Thus the different robots joints are moved with the help of python list.


