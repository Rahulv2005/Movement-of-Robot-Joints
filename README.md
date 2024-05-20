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
```python
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
![image](https://github.com/Rahulv2005/Movement-of-Robot-Joints/assets/152600335/b73ff018-909f-4e25-8ba4-c17b0a1fe77e)

</br>
</br>
</br>
</br>



### 2. robot.driveJoints(0,0,0,0,0,0)
![image](https://github.com/Rahulv2005/Movement-of-Robot-Joints/assets/152600335/addf903a-5be8-4637-a631-850e629975a4)

</br>
</br>
</br>
</br>
                



### 3. Movement of Joint1
![Screenshot 2024-05-20 164356](https://github.com/Rahulv2005/Movement-of-Robot-Joints/assets/152600335/e0d735f0-a348-4810-89e7-3adedb81497f)

</br>
</br>
</br>
</br>


### 3. Movement of Joint2
![Screenshot 2024-05-20 164543](https://github.com/Rahulv2005/Movement-of-Robot-Joints/assets/152600335/e8b8be6b-7b07-4b78-908b-7ac9fbc68e1e)

</br>
</br>
</br>
</br>

### 3. Movement of Joint3
![Screenshot 2024-05-20 164639](https://github.com/Rahulv2005/Movement-of-Robot-Joints/assets/152600335/6f4065af-2eca-4f1f-8883-1d5feb67aad9)

</br>
</br>
</br>
</br>

## Result 
Thus the different robots joints are moved with the help of python list.


