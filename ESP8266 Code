#define BLYNK_PRINT Serial
#define BLYNK_TEMPLATE_ID "TMPL7G1etx28"
#define BLYNK_DEVICE_NAME "Nurse"

#include<ESP8266WiFi.h>
#inclde<BlynkSimpleEsp8266.h>

char auth[] = "{Your_Details}";

char ssid[] = "{Your_Details}";
char pass[] = "{Your_Details}";

int IN1 = 2;
int IN2 = 0;
int IN3 = 4;
int IN4 = 5;
int ENA = 14;
int ENB = 16;
int P1, P2, P3, P4, P5, P6, P7, P8, BASE = 0;

BLYNK_CONNECTED()
{
   Blynk.syncVirtual(V0);
   Blynk.syncVirtual(V1);
   Blynk.syncVirtual(V2);
   Blynk.syncVirtual(V3);
   Blynk.syncVirtual(V4);
   Blynk.syncVirtual(V5);
   Blynk.syncVirtual(V6);
   Blynk.syncVirtual(V7);
   Blynk.syncVirtual(V8);
}

BLYNK_WRITE(V0)
{
   P1 = param.asInt();
}
BLYNK_WRITE(V1)
{
   P2 = param.asInt();
}
BLYNK_WRITE(V2)
{
   P3 = param.asInt();
}
BLYNK_WRITE(V3)
{
   P4 = param.asInt();
}
BLYNK_WRITE(V4)
{
   P5 = param.asInt();
}
BLYNK_WRITE(V5)
{
   P6 = param.asInt();
}
BLYNK_WRITE(V6)
{
   P7 = param.asInt();
}
BLYNK_WRITE(V7)
{
   P8 = param.asInt();
}
BLYNK_WRITE(V8)
{
   BASE = param.asInt();
}

void setup()
{
  Serial.begin(9600);
  pinMode(IN1, OUTPUT);
  pinMode(IN2, OUTPUT);
  pinMode(IN3, OUTPUT);
  pinMode(IN4, OUTPUT);
  pinMode(ENA, OUTPUT);
  pinMode(ENB, OUTPUT);

  Blynk.begin(auth, ssid, pass);

  Blynk.virtualWrite(V0, 0);
  Blynk.virtualWrite(V1, 0);
  Blynk.virtualWrite(V2, 0);
  Blynk.virtualWrite(V3, 0);
  Blynk.virtualWrite(V4, 0);
  Blynk.virtualWrite(V5, 0);
  Blynk.virtualWrite(V6, 0);
  Blynk.virtualWrite(V7, 0);
  Blynk.virtualWrite(V8, 0);
}

void forward()
{
  digitalWrite(ENA, HIGH);
  digitalWrite(ENB, HIGH);
  digitalWrite(IN1, HIGH);
  digitalWrite(IN2, LOW);
  digitalWrite(IN3, HIGH);
  digitalWrite(IN4, LOW);
}

void backward()
{
  digitalWrite(ENA, HIGH);
  digitalWrite(ENB, HIGH);
  digitalWrite(IN1, LOW);
  digitalWrite(IN2, HIGH);
  digitalWrite(IN3, LOW);
  digitalWrite(IN4, HIGH);
}

void right()
{
  digitalWrite(ENA, HIGH);
  digitalWrite(ENB, HIGH);
  digitalWrite(IN1, HIGH);
  digitalWrite(IN2, LOW);
  digitalWrite(IN3, LOW);
  digitalWrite(IN4, HIGH);
}

void left()
{
  digitalWrite(ENA, HIGH);
  digitalWrite(ENB, HIGH);
  digitalWrite(IN1, LOW);
  digitalWrite(IN2, HIGH);
  digitalWrite(IN3, HIGH);
  digitalWrite(IN4, LOW);
}

void rukh()
{
  digitalWrite(ENA, LOW);
  digitalWrite(ENB, LOW);
  digitalWrite(IN1, LOW);
  digitalWrite(IN2, LOW);
  digitalWrite(IN3, LOW);
  digitalWrite(IN4, LOW);
}

void loop()
{
  Blynk.run();

  if(P1 == 1)
  {
    forward();
    delay(10000);
    right();
    delay(300);
    forward();
    delay(2000);
    rukh();
    delay(10000);
    backward();
    delay(2000);
    right();
    delay(300);
    forward();
    delay(10000);
    rukh();
    right();
    delay(500);
    rukh();
    P1 = 0;
  }
  else if(P2 == 1)
  {
    forward();
    delay(10000);
    left();
    delay(300);
    forward();
    delay(2000);
    rukh();
    delay(10000);
    backward();
    delay(2000);
    left();
    delay(300);
    forward();
    delay(10000);
    rukh();
    right();
    delay(500);
    rukh();
    P2 = 0;
  }
  else if(P3 == 1)
  {
    forward();
    delay(7500);
    right();
    delay(300);
    forward();
    delay(2000);
    rukh();
    delay(10000);
    backward();
    delay(2000);
    right();
    delay(300);
    forward();
    delay(7500);
    rukh();
    right();
    delay(500);
    rukh();
    P3 = 0;
  }
  else if(P4 == 1)
  {
    forward();
    delay(7500);
    left();
    delay(300);
    forward();
    delay(2000);
    rukh();
    delay(10000);
    backward();
    delay(2000);
    left();
    delay(300);
    forward();
    delay(7500);
    rukh();
    right();
    delay(500);
    rukh();
    P4 = 0;
  }
  else if(P5 == 1)
  {
    forward();
    delay(5000);
    right();
    delay(300);
    forward();
    delay(2000);
    rukh();
    delay(10000);
    backward();
    delay(2000);
    right();
    delay(300);
    forward();
    delay(5000);
    rukh();
    right();
    delay(500);
    rukh();
    P5 = 0;
  }
  else if(P6 == 1)
  {
    forward();
    delay(5000);
    left();
    delay(300);
    forward();
    delay(2000);
    rukh();
    delay(10000);
    backward();
    delay(2000);
    left();
    delay(300);
    forward();
    delay(5000);
    rukh();
    right();
    delay(500);
    rukh();
    P6 = 0;
  }
  else if(P7 == 1)
  {
    forward();
    delay(2500);
    right();
    delay(300);
    forward();
    delay(2000);
    rukh();
    delay(10000);
    backward();
    delay(2000);
    right();
    delay(300);
    forward();
    delay(2500);
    rukh();
    right();
    delay(500);
    rukh();
    P7 = 0;
  }
  else if(P8 == 1)
  {
    forward();
    delay(2500);
    left();
    delay(300);
    forward();
    delay(2000);
    rukh();
    delay(10000);
    backward();
    delay(2000);
    left();
    delay(300);
    forward();
    delay(2500);
    rukh();
    right();
    delay(500);
    rukh();
    P1 = 0;
  }
}
    
