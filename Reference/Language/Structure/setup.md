setup()
========
원문은 [여기](https://www.arduino.cc/en/Reference/Setup)서 확인할 수 있습니다.


The setup() function is called when a sketch starts. Use it to initialize variables, pin modes, start using libraries, etc. The setup function will only run once, after each powerup or reset of the Arduino board.

setup() 함수는 sketch가 시작될때 호출되는 함수에요. 우리는 이것을 변수와 핀모드를 초기화하거나 라이브러리를 사용하고 싶을 때 사용합니다. setup() 함수는 아두이노 보드를켤 때나 리셋하고나서 딱 한번만 작동해요.


Example
--------

'''
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
 '''


[Reference Home](https://www.arduino.cc/en/Reference/HomePage)


Corrections, suggestions, and new documentation should be posted to the Forum.

The text of the Arduino reference is licensed under a Creative Commons Attribution-ShareAlike 3.0 License. Code samples in the reference are released into the public domain.
아두이노 레퍼건스는 크리에이티브 커먼즈3.0 (저작자 표시-동일조건 변경 허락) 라이센스를 준수합니다. 
