# BreathingLight
LED呼吸燈  
![image](https://github.com/wesley4406/BreathingLight/blob/main/ezgif.com-video-to-gif.gif)

***
```c++
int value=255;  
int x=-15;  
  
void setup() {   
pinMode(3,OUTPUT);   
}  
  
void loop() {   
if (value<=0 || value>=255) x=-x;   
analogWrite(3,value);   
delay(10);   
value=value-x;  
}  
```
***
