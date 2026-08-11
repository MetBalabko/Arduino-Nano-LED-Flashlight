
void setup()
{
  pinMode(4, INPUT);
  pinMode(6, OUTPUT);
  pinMode(5, OUTPUT);
  pinMode(8, OUTPUT);
  pinMode(9, OUTPUT);
  pinMode(7, OUTPUT);
  pinMode(10, OUTPUT);
  pinMode(2, INPUT);
  pinMode(3, INPUT);
}

void loop()
{
  if (digitalRead(4))
  {
    digitalWrite(6, HIGH);
    digitalWrite(5, HIGH);
    digitalWrite(8, LOW);
    digitalWrite(9, LOW);
    digitalWrite(7, LOW);
    digitalWrite(10, LOW);
  }
  else
  {
    digitalWrite(6, LOW);
    digitalWrite(5, LOW);
  }
  if (digitalRead(2))
  {
    digitalWrite(7, HIGH);
    digitalWrite(10, HIGH);
    digitalWrite(6, LOW);
    digitalWrite(5, LOW);
    digitalWrite(7, LOW);
    digitalWrite(10, LOW);
    digitalWrite(7, LOW);
    digitalWrite(10, LOW);
  }
  else
  {
    digitalWrite(7, LOW);
    digitalWrite(10, LOW);
  }
  if (digitalRead(3))
  {
    digitalWrite(8, HIGH);
    digitalWrite(9, HIGH);
    digitalWrite(6, LOW);
    digitalWrite(5, LOW);
    digitalWrite(7, LOW);
    digitalWrite(10, LOW);
  }
  else
  {
    digitalWrite(8, LOW);
    digitalWrite(9, LOW);
  }
}

