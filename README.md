# Robo_Ant
The ROBO_ANT is an autonomous robot designed using Hardware Description Language (HDL). It features two hands, right_hand and left_hand, and its movement and decision-making are controlled by a Finite State Machine (FSM). 

States and Behavior

State1 - Lost in Space:
At the beginning, the robot is lost in space.
It will move forward until it touches anything, or else it will transition to State2.

State2 - Rotate Anti-Clockwise:
When either of its hands touches an object, the robot will take a left turn (angle to be set).
If no object is touched, it will transition to State3.

State3 - Look for Wall1:
The robot will take a right turn and move forward until its right hand touches something.
If nothing is touched, it will transition to State4.

State4 - Look for Wall2:
The robot will take a left turn and move forward until its right hand touches an object while its left hand does not.
If neither hand touches an object, it will return to State3.
If the left hand touches an object, it will transition back to State2.

Motivation behind the creation of this project: https://www.youtube.com/playlist?list=PLUl4u3cNGP62WVs95MNq3dQBqY2vGOtQ2
https://www.youtube.com/watch?v=luHnuoDkAtU&t=258s
https://www.youtube.com/watch?v=Ht_tyuAWmpM&t=262s

Note: Signals need to be driven very carefully, otherwise will get wrong resuls.

