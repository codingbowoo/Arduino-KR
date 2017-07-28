원문은 [여기](https://www.arduino.cc/en/Reference/Setup)에서 확인할 수 있습니다.


setup()
========


The setup() function is called when a sketch starts. Use it to initialize variables, pin modes, start using libraries, etc. The setup function will only run once, after each powerup or reset of the Arduino board.

setup() 함수는 sketch가 시작될 때 호출되는 함수에요. 변수와 핀모드를 초기화하거나 라이브러리를 사용하고 싶을 때 사용합니다. 이 setup() 함수는 아두이노 보드를 켤 때나 리셋한 다음에  딱 한번만 작동해요.

 


Example
--------


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
    



 
 
* * *

Corrections, suggestions, and new documentation should be posted to the [Forum](https://forum.arduino.cc/index.php/board,23.0.html).

수정, 제안 및 새 도큐멘테이션은 [포럼](https://forum.arduino.cc/index.php/board,23.0.html)에 올려 주세요.



The text of the Arduino reference is licensed under a [Creative Commons Attribution-ShareAlike 3.0 License](https://creativecommons.org/licenses/by-sa/3.0/). Code samples in the reference are released into the public domain.

아두이노 레퍼런스는 [크리에이티브 커먼즈3.0 (저작자 표시-동일조건 변경 허락)](https://creativecommons.org/licenses/by-sa/3.0/deed.ko) 라이센스를 준수합니다. 
