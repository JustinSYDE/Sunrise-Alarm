Sunrise-Alarm
=============

************************************************
Author: Justin Wong, Varnit Grewal, Linda Wang 

Written in: C, C++

Filename: SunriseAlarm.ino
	
I hereby declare that this code is a product 
of my team's own efforts. This coded solution has
not been plagiarized from other sources and
has not been plagiarized by others.
************************************************

###Description

Code for an Arduino sunrise alarm system. The alarm consists of photo resistors, triLEDs, speakers, etc. When the alarm is on, a binary number is displayed via the LEDs. To turn of the alarm off, the user must input the correct decimal conversion of the binary number. Otherwise, the alarm works as any other normal alarm (i.e. displays time, snoozes, etc.). 


NOTE: This code uses the time library which can be downloaded from http://playground.arduino.cc/code/time.

###Instructions

    Step 0. Wire up Arduino and circuit as shown below

    Step 1. Compile & upload <SunriseAlarm.ino> and open the serial monitor
    
    Step 2. When surrounding environment is dark:
        
        1) Alarm is off
        2) Binary LEDs are off
        3) TriLEDs are on and output varies with brightness of the room
        4) System outputs the clock time 
        
    Step 3. When surrounding environment is bright (i.e. sunrise):
      
        1) Alarm is on
        2) Binary LEDs are on and display a random number (i.e. 0-7) in binary
        3) TriLEDs are off 
        
    Step 4. If snooze button is pressed:
        
        1) Alarm is off momentarily
        2) Binary LEDs are off momentarily
        3) Serial monitor shows that the system is in the snoozing state
        4) Can snooze up to 3 times in a row 
        
    Step 5. Else if an attempt is made to turn off the alarm:
    
        1) If correct decimal conversion is inputted -> alarm turns off
        2) Else if incorrect decimal conversion is inputted -> alarm remains on and user is given another chance 
        
  
### Pictures
  
  ![alt tag](https://raw.github.com/JustinSYDE/Sunrise-Alarm/master/SunriseAlarmCircuit.jpg)
