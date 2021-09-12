# 實作2-4 analogRead(), 1024解析度 (i.e.,10-bit): 

## 可變電阻 + 序列監視器與輸出
> 當你改變可變電阻的阻值(e.g., 10K-ohm)時，序列監視器輸出的數值有什麼改變? 數值又有什麼意義呢? 可試將你的想法寫在你的GitHub Page中喔! (互動4) (2021-09-12)

### 電路
![image](https://user-images.githubusercontent.com/89304181/132969373-0638b2d6-3e22-4381-8b2a-ffc59d60d6e9.png)

### 程式
````C
int sensorValue = 0;

void setup()
{
  pinMode(A0, INPUT);
  Serial.begin(9600);

}

void loop()
{
  // read the input on analog pin 0:
  sensorValue = analogRead(A0);
  // print out the value you read:
  Serial.println(sensorValue);
  delay(10); // Delay a little bit to improve simulation performance
````

## digitalRead(): 按鍵 + 序列監視器與輸出說明與介紹

### 電路
![image](https://user-images.githubusercontent.com/89304181/132969425-256d9c25-52f8-4151-96c3-ddde67833c3b.png)

### 程式
````C
int buttonState = 0;

void setup()
{
  pinMode(2, INPUT);
  Serial.begin(9600);

}

void loop()
{
  // read the input pin
  buttonState = digitalRead(2);
  // print out the state of the button
  Serial.println(buttonState);
  delay(10); // Delay a little bit to improve simulation performance
````
