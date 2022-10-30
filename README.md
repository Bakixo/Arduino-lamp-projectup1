# Arduino-lamp-projectup1
first development of my first project

#define Buton 8
#define led 10

int buton_durumu = 0;


void setup() {
  pinMode(Buton, INPUT);
  pinMode(led, OUTPUT);

}

void loop() {
 
  buton_durumu = digitalRead(Buton);

 if (buton_durumu==1){
   digitalWrite(led,HIGH);  
   delay(300);
   digitalWrite(led,LOW);
   delay(300);
 }

   
}
