원문은 [여기](https://www.arduino.cc/en/Reference/PinMode)에서 확인할 수 있습니다.


pinMode()
========


Description
-----------
Configures the specified pin to behave either as an input or an output. See the description of digital pins for details on the functionality of the pins.

As of Arduino 1.0.1, it is possible to enable the internal pullup resistors with the mode INPUT_PULLUP. Additionally, the INPUT mode explicitly disables the internal pullups.


Syntax
-------
pinMode(pin, mode)


Parameters
-----------
pin: the number of the pin whose mode you wish to set

mode: INPUT, OUTPUT, or INPUT_PULLUP. (see the digital pins page for a more complete description of the functionality.)


Returns
-------
None

Example
--------

    int ledPin = 13;                 // LED connected to digital pin 13

    void setup()
    {
        pinMode(ledPin, OUTPUT);      // sets the digital pin as output
    }

    void loop()
    {
        digitalWrite(ledPin, HIGH);   // sets the LED on
        delay(1000);                  // waits for a second
        digitalWrite(ledPin, LOW);    // sets the LED off
        delay(1000);                  // waits for a second
    }



Note
----

The analog input pins can be used as digital pins, referred to as A0, A1, etc.


See also
---------
constants
digitalWrite()
digitalRead()
Tutorial: Description of the pins on an Arduino board
 
* * *

Corrections, suggestions, and new documentation should be posted to the [Forum](https://forum.arduino.cc/index.php/board,23.0.html).

수정, 제안 및 새 도큐멘테이션은 [포럼](https://forum.arduino.cc/index.php/board,23.0.html)에 올려 주세요.



The text of the Arduino reference is licensed under a [Creative Commons Attribution-ShareAlike 3.0 License](https://creativecommons.org/licenses/by-sa/3.0/). Code samples in the reference are released into the public domain.

아두이노 레퍼런스는 [크리에이티브 커먼즈3.0 (저작자 표시-동일조건 변경 허락)](https://creativecommons.org/licenses/by-sa/3.0/deed.ko) 라이센스를 준수합니다. 
