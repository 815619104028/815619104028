### Hi there 👋

<!--
**815619104028/815619104028** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:
#include
int echoPin = 10; //pin 10 for the echo

int trigPin = 9; //pin 9 for trigger

int buzzPin = 12; //pin 12 for the buzzer

int ledRed = 6; //pin 6 for red LED

int ledGreen = 4; //pin 4 for green LED

int duration, inches, cm; // establish variables for duration of the ping, and the distance result

NewPing sonar(trigPin, echoPin, 200); //sets up the sonar function and limits distance to 200 cm

void setup() {

pinMode(ledRed, OUTPUT);

pinMode(ledGreen, OUTPUT);

pinMode(buzzPin, OUTPUT);

Serial.begin(9600); //sets up serial monitor

}

void loop() {

delay(100);

Serial.print("Ping: ");

Serial.print(sonar.ping_cm());

Serial.println("cm");

//warning

if(sonar.ping_cm()<10)

{

digitalWrite(ledRed, HIGH);

digitalWrite(ledGreen, LOW);

digitalWrite(buzzPin, HIGH);

}

//no warning

if(sonar.ping_cm()>=10)

{

digitalWrite(ledGreen, HIGH);

digitalWrite(ledRed, LOW);

digitalWrite(buzzPin, LOW);

}

}//end loop
- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
