# 1-2 在TinkerCAD開一個新的Circuit, 分別使甪R, G, B三種顏色的LED, ON (亮) 0.5秒, OFF(滅) 0.5秒, (互動3)


## 電路
![image](https://user-images.githubusercontent.com/89304181/133881427-0ec4f6e4-a9c7-4148-ac47-e952cc70750d.png)

## 程式

````C
void setup()
{
  pinMode(13, OUTPUT); // RED
  pinMode(11, OUTPUT); // YELLOW
  pinMode(9, OUTPUT);  // GREEN
  
}

void loop()
{
  // turn the LED on (HIGH is the voltage level)
  digitalWrite(13, HIGH);
  digitalWrite(11, HIGH);  
  digitalWrite(9, HIGH);  
  
  delay(500); // Wait for 1000 millisecond(s)
  // turn the LED off by making the voltage LOW
  digitalWrite(13, LOW);
  digitalWrite(11, LOW);  
  digitalWrite(9, LOW);
  
  delay(500); // Wait for 1000 millisecond(s)
}
````
