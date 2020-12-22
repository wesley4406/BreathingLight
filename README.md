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
# LED.LtoR
 控制LED由左至右逐一亮滅   
  ![image](https://github.com/wesley4406/LED.LtoR/blob/main/ezgif.com-video-to-gif%20(3).gif)

  
***  
```c++
int LED = 5;  
void setup ()  
{  
for ( int i = 2 ; i < 6 ; i ++)    
pinMode(i,OUTPUT);   
}  
    
void loop ()  
{  
for ( int i = 5 ; i > 1 ; i--)   
digitalWrite (i , HIGH);  
if (LED >= 2)   
digitalWrite (LED , LOW);  
else  
LED = 6;   
LED --;  
delay(500);   
}  
```
***
