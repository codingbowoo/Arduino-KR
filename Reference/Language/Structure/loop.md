원문은 [여기](https://www.arduino.cc/en/Reference/Loop)에서 확인할 수 있습니다.


loop()
========

After creating a setup() function, which initializes and sets the initial values, the loop() function does precisely what its name suggests, and loops consecutively, allowing your program to change and respond. Use it to actively control the Arduino board.

초기값을 설정하는 setup() 함수가 작동하고 나면, loop() 함수가 이름 그대로 계속해서 반복 수행됨으로써 프로그램이 변경 또는 응답을 할 수 있게 해줍니다. loop() 함수를 아두이노 보드를 능동적으로 제어하는데 사용해보세요. 


Example
--------


	const int buttonPin = 3;

 	// setup initializes serial and the button pin
 	void setup()
 	{
		Serial.begin(9600);
		pinMode(buttonPin, INPUT);
	}

	// loop checks the button pin each time,
	// and will send serial if it is pressed
     	void loop()
    	{
       		if (digitalRead(buttonPin) == HIGH)
           		Serial.write('H');
	     	else
	         	Serial.write('L');

		delay(1000);
	}

 
 
* * *

Corrections, suggestions, and new documentation should be posted to the [Forum](https://forum.arduino.cc/index.php/board,23.0.html).

수정, 제안 및 새 도큐멘테이션은 [포럼](https://forum.arduino.cc/index.php/board,23.0.html)에 올려 주세요.



The text of the Arduino reference is licensed under a [Creative Commons Attribution-ShareAlike 3.0 License](https://creativecommons.org/licenses/by-sa/3.0/). Code samples in the reference are released into the public domain.

아두이노 레퍼런스는 [크리에이티브 커먼즈3.0 (저작자 표시-동일조건 변경 허락)](https://creativecommons.org/licenses/by-sa/3.0/deed.ko) 라이센스를 준수합니다. 
