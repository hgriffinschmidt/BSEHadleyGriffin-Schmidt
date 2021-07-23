# Robot Arm
Using an Arduino Uno and Servo Motors, the arm can make controlled movements and complete certain tasks within the range of the movements.

| Hadley Griffin-Schmidt | Urban School of San Francisco | Mechanical Engineering | Rising Senior |
|:--:|:--:|:--:|:--:|

![Headstone Image](https://bluestampengineering.com/wp-content/uploads/2016/05/improve.jpg)

  
# Final Milestone
My final milestone is the increased reliability and accuracy of my robot. I ameliorated the sagging and fixed the reliability of the finger. As discussed in my second milestone, the arm sags because of weight. I put in a block of wood at the base to hold up the upper arm; this has reverberating positive effects throughout the arm. I also realized that the forearm was getting disconnected from the elbow servo’s horn because of the weight stress on the joint. Now, I make sure to constantly tighten the screws at that joint. 

[![Final Milestone](https://res.cloudinary.com/marcomontalbano/image/upload/v1612573869/video_to_markdown/images/youtube--F7M7imOVGug-c05b58ac6eb4c4700831b2b3070cd403.jpg )](https://www.youtube.com/watch?v=F7M7imOVGug&feature=emb_logo "Final Milestone"){:target="_blank" rel="noopener"}

<img src="carbon.png" width=500 align=center style="float:right; padding-right:10px">

# Second Milestone
For my second milestone I decided to focus on potentiometers. Noticing that the potentiometers would be essential for the final product - controlling the movement of the specficic joints of the arm - I spent my time learning how to use imputs and convert them to outputs with the arduino. To store the initial imputs, I had the arduino read the signal coming from the potentiometer using analogRead() - from 0 to 1023 - and store it in a previously defined varible. To use the analogRead() function, I had to hook up the potentiometer to one of the analog pins. Once the imput value had been stored, the next step was mapping out the value to the range of the motor. Being that the motor only rotates between 0 and 179 and the value of the potentiometer ranged from 0 to 1023, the map() funtion allowed me to scale down the values so the  turn of the potentiometer would correlate directly with the servo rotation. To store this new value I used a different "output value", also perviosuly defined. Finally, now that the value has been converted, the arduino sends the output value to the servo using [servo].write() and the servo turns accordingly.

[![Hadley Second Milestone Video](https://res.cloudinary.com/marcomontalbano/image/upload/v1626900543/video_to_markdown/images/youtube--Pg5RJ3HaIMg-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://www.youtube.com/watch?v=Pg5RJ3HaIMg "Hadley Second Milestone Video"){:target="_blank" rel="noopener"}

# First Milestone 
My first milestone was getting comfortable with Arduino, LEDs, and Servo Motors. Being new to circuitry and coding, it was important to me that before jumping into the project specs, I take a deep dive into the how and why. Starting with Blink, a simple code which blinks the led on the arduino on and off, I became comfortable with digitalWrite(), learning how to control two outputs (HIGH or LOW) to turn the LED on and off. Once comforable, I then dove into outsourcing the LED. Using digital pins, I was able to get my first introduction to circutry, spefically Ohm's Law and how to manipulate restisotrs to allow for the correct amount of current. From there, I moved on to  ~PWM pins which generate a steady rectangular wave to allow incrimental results through digital means using, for example the analogWrite() function. Rather than being either on or off, the fucntion can output anything between the allowed range (ie 0 to 255 for an LED) allowing for much more specific control. Among the new possiblites using PWM pins is the abilty to control the brightness of an LED and the rotation of a Servo Motor. Using a for() loop, I correlated two servo motors turn torwards 180 to the brightness of an LED, and its turn back to a corresponding dimming effect, using everything I have learned thus far.

[![Hadley First Milestone Video](https://res.cloudinary.com/marcomontalbano/image/upload/v1626463562/video_to_markdown/images/youtube--ouI9OeCi77s-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://www.youtube.com/watch?v=ouI9OeCi77s "Hadley First Milestone Video"){:target="_blank" rel="noopener")
