# Lesson #1: Debugging Your Code

### Lesson Plan:
1. Watch the lesson plan video below
2. Follow the instructions to complete the assignment.  Be sure to complete all the steps!
3. Show or share the completed assignment with a mentor

<p align="center">
<iframe width="560" height="315" src="https://www.youtube.com/embed/Yr5yAB4Nweo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

### Code Comments
  * A code comment is a text note added to source code to provide information, usually about the function of the code.
  * A comment in Python starts with the hash character, # and extends to the end of the line.
  * An example Python comment is shown below
```python
# This entire line is a Python comment
# Comments are a great way to let other people know how your program works

# You can also use comments to remove one or more lines of code from you program.
# This can be helpful when debugging your program.
# For example, the following line starts with the hash character, # so it is a comment:
# robot.turn(90)

# Removing the hash chararcter turns it into a line of code to be executed:
robot.turn(90)
```

### Print Function: print()
  * Print function calls can be added to your code to display messages to the console.
  * In some cases, like when using the simulator or when using Visual Studio Code these can be used to display helpful information about what your code is doing.
  * Print statements are not displayed on the EV3's screen.  We'll cover how to do that in a different lesson.
  * You print text with the print function by including it in quotes like this:
```python
# A simple text print message
print("Hello World.")
```
  * Print statements can be more advanced like in the example below.
  * A plus sign, + can be used to join variables, text and other elements together.
  * The variable speed is a number and is converted to a text string for printing using the str() function
```python
# Set the variable speed equal to 200
speed = 300
# Print the value of the variable speed
print("Speed= " + str(speed) + " mm/Second")
```

### The wait() Method

### 1. In a different browser window or browser tab start the simulator: 
  * [Launch FSS FLL Simulator: LESSON 2](https://fssfll.github.io/gears/public/index.html?worldJSON=https%3A%2F%2Ffssfll.github.io%2Ffssfll%2Flesson1%2Flesson1.json)
  * Make sure you are in Python "Pybricks Mode"

...TBD STUFF...


