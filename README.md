
int tsensor;
void setup()
{
  pinMode(A2,INPUT);
  pinMode(13,OUTPUT);
  pinMode(12,OUTPUT);
}
void loop()
{
  tsensor=analogRead(A2);
  if(tsensor >=200)
  {
    digitalWrite(13,HIGH);
    tone(12,500,500);
  }
  digitalWrite(18,LOW);
}
