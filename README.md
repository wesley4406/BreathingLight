# BreathingLight
LED呼吸燈
![image](https://github.com/wesley4406/BreathingLight/blob/main/video-1608605068.mp4)

***
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
***
