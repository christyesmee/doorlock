#Keypad Simulation Script
This script simulates a dataset of varying time intervals based on the Euclidean distance between key pairs on a door lock pad. It is designed to calculate the time taken for a finger to traverse from one key to another on a keypad.

##The key factors determining these time intervals include:

The Euclidean distance between keys, measured as a straight line.
The speed at which a finger can move across the keypad.
The minimum time required for each key press to be registered.
The script employs these factors to compute the time intervals needed for a finger to move between keys. All calculated intervals are rounded for ease of analysis and interpretation.

The output is a comprehensive table that pairs each unique combination of keys with their corresponding time intervals. This table is essential for understanding the dynamics of keypress intervals in the context of the simulated door lock pad.

##Key Calculation Components:
###Speed of Finger Movement: 
This is the average speed at which a finger moves across the keypad, measured in centimeters per second. It influences the time taken to move from one key to the next.
###Minimum Press Time: 
The minimal duration required to press a key effectively, ensuring the keypress is registered.
###Time Interval Calculation:
The script calculates the time interval by dividing the Euclidean distance between keys by the finger movement speed and then adding the minimum key press time. The formula used is: (distance / speed_cm_per_sec) + min_press_time_sec.

This simulation provides insightful data that can be used for various applications, including security systems, ergonomic studies, and user interface design.