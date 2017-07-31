원문은 [여기](https://www.arduino.cc/en/Reference/PinMode)에서 확인할 수 있습니다.


pinMode()
========


Description (설명)
-----------
Configures the specified pin to behave either as an input or an output. See the description of [digital pins](https://arduino.cc/en/Rurotial/DigitalPins) for details on the functionality of the pins.

특정 핀을 입력 또는 출력으로 작용하도록 설정한다. 핀들과의 상관관계에  대한 자세한 정보는 디지털 핀의 설명을 참고하시라.

As of Arduino 1.0.1, it is possible to enable the internal pullup resistors with the mode INPUT_PULLUP. Additionally, the INPUT mode explicitly disables the internal pullups.

아두이노 1.0.1 부터는 INPUT_PULLUP 모드를 통해 내부 풀업 저항을 활성화 할 수 있다. 덧붙여 INPUT 모드는명시적으로 내부 풀업을 비활성화 한다. 


Syntax (문법)
-------
pinMode(pin, mode)


Parameters (인자)
-----------
pin: the number of the pin whose mode you wish to set
pin: 모드를 설정하고 싶은 핀의 번호

mode: INPUT, OUTPUT, or INPUT_PULLUP. (see the digital pins page for a more complete description of the functionality.)
mode: INPUT, OUTPUT 혹은 INPUT_PULLUP. (기능에 대한 더 자세한 설명은 digital pin 페이지를 참조하세요.)

Returns
-------
None
없음

Example
--------

    int ledPin = 13;                 // LED connected to digital pin 13 - LED와 13번 핀 연결 

    void setup()
    {
        pinMode(ledPin, OUTPUT);      // sets the digital pin as output- 디지털 핀을 출력핀으로 설정
    }

    void loop()
    {
        digitalWrite(ledPin, HIGH);   // sets the LED on- LED 켬
        delay(1000);                  // waits for a second- 1초 기다림
        digitalWrite(ledPin, LOW);    // sets the LED off- LED 끔
        delay(1000);                  // waits for a second- 1초 기다림
    }



Note
----

The analog input pins can be used as digital pins, referred to as A0, A1, etc.

A0, A1과 같은 아날로그 입력 핀들도 디지털 핀으로 이용할 수 있다.


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
