# FSS FLL Python Information
## Getting Started
### Using the Simulator
You don't need anything!  Just head over to the [FSS Gears Pybricks Simulator](https://fssfll.github.io/gears/public/)
### Using the EV3 Bot
Official Lego Education instructions on how to get an EV3 bot up and running with Python: 

[https://education.lego.com/en-us/product-resources/mindstorms-ev3/teacher-resources/python-for-ev3](https://education.lego.com/en-us/product-resources/mindstorms-ev3/teacher-resources/python-for-ev3)

Note there are different versions of Python available for running on the EV3.  The current recommendation is to use the Lego Education supported EV3 Micropython which is a slimmed down and simplified version Python making it easier for beginners to use.  Micropython can be paired with a dedicated Visual Studio Code extension that includes project templates and documentation.

To run on an EV3, you'll need the following:
- MicroSD Card (4GB to 32GB of type microSDHC) to store the operating system and python programs on the EV3
- MicroSD Card reader or adapter to write the OS to the MicroSD Card
- Wifi USB dongle to connect to the EV3 wirelessly using Microsoft Visual Code Studio (not required, but recommended).  
## Connecting to the EV3 Bot

- USB Cable: Wired programming of the EV3 is supported
- Wifi: Adding a USB dongle to the EV3 allows for the bot to be programmed using wifi.  Connection instructions provided below.
- Before connecting to the ev3 robot in a classrom environment it is strongly recommended to first [rename the EV3 robot](./rename.md).
  1. Insert the dongle when the bot is off 
  2. Power up the EV3 and wait for the bot to fully boot
  3. Navigate and select the "Wireless and Networks" menu option
  4. Navigate and select the "Wi-Fi" menum option
  5. If needed, select the "Powered" menu option to enable the Wifi.  The check box should be filled in once selected.
  6. Click the "Start Scan" menu option to select identify available Wifi networks
  7. Once the scan is complete, select the desired Wifi network.  This must be the same Wifi network as used by the computer used to program the EV3.
  8. Enter the Wifi password, the click "ok"
  9. Wait for the wifi to configure and associate.

- Bluetooth: Other ev3 Python users have reported that Bluetooth is not reliable and is therefore not currently recommended.

## Lessons:
- [Create Your First Python Program](./lessons/lesson1/lesson1.md) : Using the simulator write a python script to move virtual blocks into scoring areas
- [Changing Speed Using the Drivebase Settings](./lessons/drivebase_settings/drivebase_settings.md) : Use the drivebase settings to change the speed of your robot
- [Code Debugging](./lessons/debugging/debugging.md) : How to debug your python program
- [Code Loops](./lessons/loops/loops.md) : Learn how to use a code loop to perform a repeated action
- [Driving Using Code Loops](./lessons/driving_with_loops/driving_with_loops.md) : Using loops to drive on a curve and line follow
- [First Python Program on the EV3](./lesson2/lesson2.md) : Use the EV3 robot write a python script to move blocks into scoring areas
- [Using the EV3 display](./lessons/display/display.md) : Learn how to display text on the EV3 display
- TBD - Using the EV3 buttons to select a python program

## Additional How-To's:
- [Rename the EV3 Robot](./rename/rename.md) : Use SSH in Visual Studio Code to give the EV3 robot a unique name.
- [Color Sensor Calibration](./calibration/calibration.md) : Color Sensor Calibration Routine for line following

## Robot Game
- [2022 FSS FLL Spring Training Robot Game](./spring_2022/robot_game.md) : After completing all lessons students may work on the robot game.

## Code Repo
Github Repo for FSS Python code:
https://github.com/kmortime/fss_fll_python/

### Additional Details:
This simulation above is a clone of the [https://github.com/kendmaclean/gears_pybricks/](https://github.com/kendmaclean/gears_pybricks/) repository which itself is a fork of the [https://github.com/QuirkyCort/gears](https://github.com/QuirkyCort/gears) repository initially created by the great people at [https://www.aposteriori.com.sg/](https://www.aposteriori.com.sg/)
## More Resources
* [Pybricks Documentation](https://pybricks.com/ev3-micropython/index.html)
