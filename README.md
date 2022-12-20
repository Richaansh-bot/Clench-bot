# Clench-bot

# Welcome to the project!

This codebase is for a robot that is controlled by pulse width modulation (PWM) signals. The robot has four channels of input: two for the wheels, one for the gripper, and one for the base tilt.

The code is written in C++ and was developed for use with an Arduino microcontroller.

In the `setup()` function, the input and output pins are configured, and the serial communication is initialized. The `loop()` function continuously reads the input values from the four channels and maps them to a range of -255 to 255. These values are then used to control the speed of the motors and the tilt of the base.

The code also includes logic for controlling the direction of the wheels and gripper. If the input value for the wheels is 0, the wheels stop moving. If the input value is greater than 1530, the wheels move forward. If the input value is less than 1470, the wheels move backward. The same logic is applied to the gripper. If the input value for the gripper is 0, the gripper stops moving. If the input value is greater than 1530, the gripper closes. If the input value is less than 1470, the gripper opens.

Finally, the code includes logic for controlling the tilt of the base. If the input value for the base tilt is 0, the base remains stationary. If the input value is greater than 0, the base tilts to the right. If the input value is less than 0, the base tilts to the left.

## Getting started

To use this code, you will need to connect the appropriate hardware to your Arduino microcontroller and upload the code using the Arduino Integrated Development Environment (IDE). You will also need to provide the necessary PWM signals to control the robot.

## Questions or feedback

If you have any questions or need further assistance, please don't hesitate to reach out. We are here to help!
