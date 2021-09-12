# Lab2-3


## Circuit
![image](https://user-images.githubusercontent.com/89304181/132971172-444a94f8-9389-49f1-8156-be9a77e650e6.png)


## Code
````C
int brightness = 0;
int R = 9;
int G = 11;
int B = 10;

void setup()
{
  pinMode(R, OUTPUT);
  pinMode(G, OUTPUT);  
  pinMode(B, OUTPUT);  
  
  Serial.begin(9600); // Enable serial function
}

void loop()
{
  Serial.println("Demo Start");
// RED
  for (brightness = 0; brightness <= 255; brightness += 5) {
    analogWrite(R, brightness);
    delay(50); // Wait for 30 millisecond(s)
  }
  for (brightness = 255; brightness >= 0; brightness -= 5) {
    analogWrite(R, brightness);
    delay(50); // Wait for 30 millisecond(s)
  }
  delay(1000); //1000ms = 1s
  
// GREEN
  for (brightness = 0; brightness <= 255; brightness += 5) {
    analogWrite(G, brightness);
    delay(50); // Wait for 30 millisecond(s)
  }
  for (brightness = 255; brightness >= 0; brightness -= 5) {
    analogWrite(G, brightness);
    delay(50); // Wait for 30 millisecond(s)
  }  
  delay(1000); //1000ms = 1s
  
// BLUE
  for (brightness = 0; brightness <= 255; brightness += 5) {
    analogWrite(B, brightness);
    delay(50); // Wait for 30 millisecond(s)
  }
  for (brightness = 255; brightness >= 0; brightness -= 5) {
    analogWrite(B, brightness);
    delay(50); // Wait for 30 millisecond(s)
  }  
  delay(1000); //1000ms = 1s  delay(1000); //1000ms = 1s  
  Serial.println("Demo Complete");  

}

````
