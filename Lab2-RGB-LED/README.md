# Brightness Comparison 


## Circuit
![image](https://user-images.githubusercontent.com/89304181/132114978-7ff65f44-1de6-4c21-b748-5c360ac44928.png)


## Code
````C
int R = 9;
int G = 10;
int B = 11;

int DR = 2;
int DG = 4;
int DB = 7;

int level = 64;
void setup()
{
  pinMode(R, OUTPUT);
  pinMode(G, OUTPUT);
  pinMode(B, OUTPUT);  
  
  pinMode(DR, OUTPUT);
  pinMode(DG, OUTPUT);
  pinMode(DB, OUTPUT);   
}

void loop()
{
	analogWrite(R, level);
	analogWrite(G, 0);
	analogWrite(B, 0);  
  
	digitalWrite(DR, 1);
	digitalWrite(DG, 0);
	digitalWrite(DB, 0);  
  
  	delay(1000);
  
	analogWrite(R, 0);
	analogWrite(G, level);
	analogWrite(B, 0);
  
	digitalWrite(DR, 0);
	digitalWrite(DG, 1);
	digitalWrite(DB, 0);
  
  	delay(1000);
	analogWrite(R, 0);
	analogWrite(G, 0);
	analogWrite(B, level);
  
	digitalWrite(DR, 0);
	digitalWrite(DG, 0);
	digitalWrite(DB, 1);  
  
    delay(1000);
}

````
