
**Troubleshooting and Debug Tips**

* You won't be able to connect to the EV3 if it is currently running a program.  You must stop the program first and then try to connect.
* Python is very picky about indentation.  Code must have the same indentation level, code within a method or while loop must be indented further.
* It is a good practice to use the "run and debug" operation which can be started by pressing the "F5" key.
* The "OUTPUT" window will display errors in your code.  Usually it is a good idea to start at the bottom of the Traceback messages and work backwards.  Here's an example:
* Wifi USB adapters can eliminate the need to plug a cable onto the EV3 to download code and greatly speed up design iteration.  I've found the CanaKit USB Wifi Adapter works although it is not officially listed.  Not all USB Wifi adapaters will work!  When connected with Wifi and using the "run and debug" mode, you will see print messages in the Visual Studio Code window.  This can be very hepful to get real-time feedback about what the code is doing as the robot is running on the table. 
* If the EV3 "hangs" and is no longer responsive to the buttons it must be restarted.  This can be done by pressing and holding the center button and the back button at the same time.  If the EV3 frequently hangs, the MicroSD card may need to be re-imaged.  We've seen re-imaging the MicroSD cards solve the hang problem but don't yet understand why.