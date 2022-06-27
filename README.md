# Program 1
void setup()
{
  pinMode(13, OUTPUT);
}
void loop()
{
  digitalWrite(13, HIGH);
  delay(1000);
  delay(1000);
  digitalWrite(13, LOW);
  delay(1000);
}

OUTPUT<br>
![image](https://user-images.githubusercontent.com/97939284/175920829-41e168c8-5a6c-4a1a-93a4-1fdff569c922.png)

# Program 2
void setup()<br> 
{
 pinMode(13, OUTPUT);<br>
 pinMode(12, OUTPUT);<br>
 pinMode(11, OUTPUT);<br>
}<br>

void loop()<br>
{
  digitalWrite(13, HIGH);<br>
  delay(1000);<br>
  digitalWrite(13, LOW);<br>
  delay(1000);<br>
  digitalWrite(12, HIGH);<br>
  delay(1000);<br>
  digitalWrite(12, LOW);<br>
  delay(1000);<br>
  digitalWrite(11, HIGH);<br>
  delay(1000);<br>
  digitalWrite(11, LOW);<br>
  delay(1000);<br>
}<br>

OUTPUT:<br>

# Program 3

void setup() 
{
  pinMode(11, OUTPUT);
  pinMode(10, OUTPUT);
  pinMode(9, OUTPUT);
}
void loop()
{
  displayColor(0b100);
  delay(1000);
  displayColor(0b010);
  delay(1000);
  displayColor(0b001);
  delay(1000);
  displayColor(0b101);
  delay(1000);
  displayColor(0b011);
  delay(1000);
  displayColor(0b110);
  delay(1000);
  displayColor(0b111);
  delay(1000);
}
void displayColor(byte color)
{
  digitalWrite(11,!bitRead(color,2));
  digitalWrite(10,!bitRead(color,1));
  digitalWrite(9,!bitRead(color,0));
}
