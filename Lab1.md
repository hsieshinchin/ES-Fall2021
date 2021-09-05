# 嵌入式系統 - 實作1

## 1.1 在TinkerCAD開一個新的Circuit, 加上一個外部的LED, 並且ON (亮) 1秒, OFF(滅) 1秒
### 電路圖與程式
![image](https://user-images.githubusercontent.com/55008636/131115066-2349e7f4-28ad-4e71-a5f1-d4e0a70c52a6.png)

## 1.2 在TinkerCAD開一個新的Circuit, 分別使甪R, G, B三種顏色的LED, ON (亮) 0.5秒, OFF(滅) 0.5秒

### 電路圖
![image](https://user-images.githubusercontent.com/55008636/132095940-bcb758b4-fafb-4d27-b724-a822ddcc520a.png)

### 程式
````C

/*
  This program blinks pin 13 of the Arduino (the
  built-in LED)
*/

void setup()
{
  pinMode(13, OUTPUT);
  pinMode(11, OUTPUT);
  pinMode(9, OUTPUT);  
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


````C
/*
  This program blinks pin 13 of the Arduino (the
  built-in LED)
*/

void setup()
{
  pinMode(13, OUTPUT);
  pinMode(11, OUTPUT);
  pinMode(9, OUTPUT);  
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

## 1.3 3 在TinkerCAD開一個新的Circuit, 分別使甪R, G, B三種顏色的LED, 讓LED ON, OFF的順序為R >> G >> B >> G >> R .... 無限循環

### 電路圖
![image](https://user-images.githubusercontent.com/55008636/132096446-6d876662-1646-402b-b613-54848e768b1d.png)

### 程式
````C
void setup()
{
  pinMode(13, OUTPUT);
  pinMode(11, OUTPUT);
  pinMode(9, OUTPUT);
}

void loop()
{
  // turn the LED on (HIGH is the voltage level)
  digitalWrite(13, HIGH);
  digitalWrite(11, LOW);
  digitalWrite(9, LOW);
  delay(500); // Wait for 1000 millisecond(s)
  // turn the LED off by making the voltage LOW
  digitalWrite(13, LOW);
  digitalWrite(11, HIGH);
  digitalWrite(9, LOW);
  delay(500); // Wait for 1000 millisecond(s)
  // turn the LED off by making the voltage LOW
  digitalWrite(13, LOW);
  digitalWrite(11, LOW);
  digitalWrite(9, HIGH);
  delay(500); // Wait for 1000 millisecond(s)  
  digitalWrite(13, LOW);
  digitalWrite(11, HIGH);
  digitalWrite(9, LOW);  
  delay(500); // Wait for 1000 millisecond(s)  
}
````
