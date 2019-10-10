# Use an Arduino to make a LED light blink in the SOS distress pattern
In this lab you will build a circuit with one LED and one resistor. You will then write a program for the Arduino using the [Scratch for Arduino](http://s4a.cat/) language. The program will blink the LED light repeatedly in the [SOS distress signal](https://en.wikipedia.org/wiki/SOS) of three short blinks, three long blinks, three more short blinks and then a pause.  The SOS distress signal is used to indicate an emergency and that someone needs help.    
![](SOSblink.gif)   
### Step 1: Start the Scratch for Arduino program
You can find it by clicking on the Start Menu at the bottom left of the screen and choosing *S4A*. Since the Arduino has not been connected yet, the S4A program should display a "Searching Board" message.

### Step 2: Connect the Arduino with a USB cable
Connect the Arduino to the computer with a USB cable. The "Searching Board" message should disappear. You can test the connection by dragging a *digital 13 on* block to scripts and clicking on it.
![](SOSblink1.PNG)   
The built in blue LED near pin 13 (shown below) on the Arduino should light up.    
![](RedBoardLEDpin13.png)   
To turn the LED off, drag a *digital 13 off* block to scripts and click on it. 

### Step 3: Build and test the LED circuit
You will need the following parts:
- 1 LED with **two wires** (called "leads") of any color. (**NOT** the white LED with **4** leads)
- 1 330Ω ("Ohm") resistor (NOT the 10KΩ resistor, see picture below)
- 2 jumper wires (the color of the wires doesn't matter, but you may find it convenient to use the same colors in the wiring diagram below)   
![](SOSblink2.png)
Connect the parts as shown below. Note that the direction of the resistor and jumper wires doesn't matter, but the LED must be connected so that the flat side with the shorter lead is connected to ground (labeled **GND** on the Arduino board). The longer lead of the LED should be connected to the resistor and the resistor should connect to pin 13.   
![](SOSblink3.png)   
You can test your circuit by moving the jumper wire from pin 13 on the Arduino to the the 5V POWER pin as shown below. The LED should light up if the Arduino is plugged in and you have built the circuit correctly. If the LED is dimly lit, check to make sure you used the correct resistor. Once you have tested your circuit, move the jumper wire back to pin 13.   
![](SOSblink4.png)   
### Step 4: Write some Scratch code
To start, drag the following blocks into Scripts:
- 1 *digital 13 on* block from the *Motion* tab
- 1 *digital 13 off* block from the *Motion* tab
- 2 *wait 1 secs* blocks from the *Control* tab
- 1 *forever loop* block from the *Control* tab    

Arrange the blocks so that they snap together as shown below. Click on the blocks to start the program. Your LED should blink on and off.         
![](SOSblink5.png)   
### Step 5: Save your program to *My Projects*
Choose *File | Save* and name your project something like `SOSblink`. Save your project to your *My Projects* folder and click *Ok*.   
![](SOSblink6.png)   
### Step 6: Finish the program
The SOS pattern is 3 short blinks, 3 long blinks, 3 short blinks with a pause before the pattern repeats. One finished program used the following blocks:
- 1 *forever loop* block
- 9 *digital on* blocks
- 9 *digital off* blocks
- 18 *wait* blocks

Optional: You can use 3 *repeat* blocks to reduce duplication in the code. You can also create two *variable* blocks for the long and short wait times.

### Step 7: Submit the finished program
Have your teacher or a TA verify that you have a working program. Then, submit your finished program by uploading the `SOSblink.sb` file to Google classroom. You should be able to find it in *My Documents | Scratch Projects* as shown below.    
![](SOSblink7.png)   
If you worked with a partner, each partner should submit a copy of the finished program to Google classroom.   

