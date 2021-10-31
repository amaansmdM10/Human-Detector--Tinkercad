 #include <LiquidCrystal.h>

// initialize the library with the numbers of the interface pins
LiquidCrystal lcd(12, 11, 5, 4, 3, 2);

void setup() {
  // set up the LCD's number of columns and rows:
  lcd.begin(16, 2);
  // Print a message to the LCD.
 
  pinMode(8, OUTPUT);
  pinMode(9, OUTPUT);
  pinMode(A0,INPUT);
  Serial.begin(9600);
  
}

void loop() {
  // set the cursor to column 0, line 1
  // (note: line 1 is the second row, since counting begins with 0):
  lcd.setCursor(0, 1);
  int x=digitalRead(A0);
  Serial.print(x);
  if(x==HIGH){
    digitalWrite(8,HIGH);
    digitalWrite(9,HIGH);
    lcd.setCursor(0, 0);
    lcd.print("Caught YOu");
    delay(500);
    lcd.clear();
  }
  else if(x==LOW){
    digitalWrite(8,LOW);
    digitalWrite(9,LOW);
    lcd.setCursor(0, 0);
    lcd.print("NO ONe there ");
    delay(500);
  lcd.clear();}
  // print the number of seconds since reset:
  
  
}
