setup()
========

The setup() function is called when a sketch starts. Use it to initialize variables, pin modes, start using libraries, etc. The setup function will only run once, after each powerup or reset of the Arduino board.

Example


 int buttonPin = 3;

 void setup()
 {
   Serial.begin(9600);
     pinMode(buttonPin, INPUT);
     }

     void loop()
     {
       // ...
       }

       Reference Home

       Corrections, suggestions, and new documentation should be posted to the Forum.

       The text of the Arduino reference is licensed under a Creative Commons Attribution-ShareAlike 3.0 License. Code samples in the reference are released into the public domain.

