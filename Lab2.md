# 嵌入式系統 - 實作2: 會呼吸的RGB LED,  按鍵控制, 狀態輸出

## 實作2-1, analogWrite(): 並且觀查LED亮度變化是否有像"呼吸的效果"和示波器的波形有什麼關連性? (互動1), (2021-09-05)

![image](https://user-images.githubusercontent.com/89304181/132113065-8d66f2a8-38d7-47c6-a3c5-56d7c54536a2.png)


## 實作2-2, RGB LED燈全彩模組, 分別讓LED輪流表現正紅、正綠、正藍，三個顏色，時間間隔1秒鐘。並且觀查LED顏色和波形或是電壓有什麼關連性? 可將個人說明在更新GitHub時一起加入. (互動2), (2021-09-05)
![image](https://user-images.githubusercontent.com/89304181/132113030-13751225-740f-4d4b-bdf3-022da9f9302e.png)

```C

int R = 9;
int G = 10;
int B = 11;

void setup()
{
  pinMode(R, OUTPUT);
  pinMode(G, OUTPUT);
  pinMode(B, OUTPUT);  
}

void loop()
{
	analogWrite(R, 255);
	analogWrite(G, 0);
	analogWrite(B, 0);
  	delay(1000);
	analogWrite(R, 0);
	analogWrite(G, 255);
	analogWrite(B, 0);
  	delay(1000);
	analogWrite(R, 0);
	analogWrite(G, 0);
	analogWrite(B, 255);
  	delay(1000);  
}

````
