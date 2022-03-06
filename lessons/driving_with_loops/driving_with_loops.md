# Driving Using Loops

## Lesson Plan:
1. Watch the lesson plan video below
2. Read the informaion and follow the instructions to complete the assignment.  Be sure to complete all the steps!
3. Show or share the completed assignment with a mentor

<p align="center">
TBD
</p>

## Loops can be used for robot moevement
  * Use loops to drive on an curved path for specific distance  
  * Use loops to line follow

### Driving on a curved path
 * Tank turns (turning in place without moving) is a great tool, but what if you needed to drive on a curved path?
 * The robotics **drive(drive_speed, turn_rate)** method can be used to drive on a curved path but notice that it does not have distance as an input parameter.
 * Using the **drive()** method by itself will make your robot drive in circles until you press the stop button or the batteries run out!
 * Using the **drive()** method inside a while loop allows you to control the distance.
 * Let's try an example.
 * Start the [FSS FLL Simulator](https://fssfll.github.io/gears/public/index.html?worldJSON=https%3A%2F%2Ffssfll.github.io%2Ffssfll%2Flessons%2Flesson1%2Flesson1.json)
```python
# Create and define distance, speed, and turn variables
# to control how fast the robot moves, how sharp it turns, and how far it will go.
speed = 75
turn = -25
distance = 250

# While the robot.distance() is less than or equal to the variable 'distance' stay in the while loop
while (robot.distance() <= distance):
  robot.drive(speed,turn)

# robot.drive() goes on forever, even after the while loop ends.
# You need to stop the robot after exiting the while loop
robot.stop()
```

### Line following
 * The same approach can be used to follow a line using a color sensor and a proporitional feedback loop.


```python
# Create and define a proportional gain variable for line following
pd = -0.8

# Create and define distance and speed variables
distance = 1000
speed = 100

while (robot.distance() <= distance):
  # The turn direction is equal to the gain x (color sensor value - 50)
  turn_direction = pd * (color_sensor_in1.reflection() - 50)
  robot.drive(speed,turn)

# Stop the robot
robot.stop()
```



## Now it is your turn!

### 1. In a different browser window or browser tab start the simulator: 

  * [Launch FSS FLL Simulator: LESSON 2](https://fssfll.github.io/gears/public/index.html?worldJSON=https%3A%2F%2Ffssfll.github.io%2Ffssfll%2Flessons%2Flesson1%2Flesson1.json)
  * Make sure you are in Python "Pybricks Mode"

### 2. Copy in the example program below and try out the already completed "Part 1"

### 3. Follow the instructions in the code comments below to complete "Part 2" of the assignment

```python
#!/usr/bin/env pybricks-micropython

# Import the necessary libraries
import math
import time
from pybricks.parameters import *
from pybricks.hubs import EV3Brick
from pybricks.ev3devices import *
from pybricks.tools import wait
from pybricks.robotics import DriveBase

# Create the sensors and motors objects
ev3 = EV3Brick()

motorB = Motor(Port.B)
motorC = Motor(Port.C)
left_motor = motorB
right_motor = motorC

color_sensor_in1 = ColorSensor(Port.S1)


robot = DriveBase(left_motor, right_motor, wheel_diameter=56, axle_track=108)
robot.settings(straight_speed=200, straight_acceleration=100, turn_rate=100, turn_acceleration=100)

################################################
# Here is where your code starts
################################################

#-----------------------------------------------------------
#                           PART 1
#
# Example of using print, comments, and the wait() method
#-----------------------------------------------------------
# Example print message
print("Hello World!")

# Pause the program for half a second
print("Pausing the program for half a second")
wait(500)

# Continuing the program
print("The program resumes...")

#-----------------------------------------------------------
#                           PART 2
#
# Now it is your turn to add on to the program.
# Use the robot.straight() methods to move foward,
# then wait for 5 seconds, then move backwards to return home.
# Use print() to display on the console what your robot is doing
#-----------------------------------------------------------


# Use print() to say your robot will move forward

# Use robot.straight() to move forward

# Use print() to say you are waiting for 5 seconds

# Use wait() to pause for 5 seconds.  Try commenting out the wait() to remove the pause.

# Use print() to say your robot will move backwards

# Use robot.straight() to move backwards

# Use print() to say mission accomplished and you've returned to base!


```


