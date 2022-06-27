# Program 1
void setup()<br>
{<br>
  pinMode(13, OUTPUT);<br>
}<br>
void loop()<br>
{
  digitalWrite(13, HIGH);<br>
  delay(1000);<br>
  delay(1000);<br>
  digitalWrite(13, LOW);<br>
  delay(1000);<br>
}<br>

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
void setup()<br> 
{<br>
  pinMode(11, OUTPUT);<br>
  pinMode(10, OUTPUT);<br>
  pinMode(9, OUTPUT);<br>
}<br>
void loop()<br>
{<br>
  displayColor(0b100);<br>
  delay(1000);<br>
  displayColor(0b010);<br>
  delay(1000);<br>
  displayColor(0b001);<br>
  delay(1000);<br>
  displayColor(0b101);<br>
  delay(1000);<br>
  displayColor(0b011);<br>
  delay(1000);<br>
  displayColor(0b110);<br>
  delay(1000);<br>
  displayColor(0b111);<br>
  delay(1000);<br>
}<br>
void displayColor(byte color)<br>
{
  digitalWrite(11,!bitRead(color,2));<br>
  digitalWrite(10,!bitRead(color,1));<br>
  digitalWrite(9,!bitRead(color,0));<br>
}<br>

OUPUT:<br>


