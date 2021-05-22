#include<LiquidCrystal_I2C.h>
LiquidCrystal_I2C lcd(0x27, 16 , 2);

int hour=0;
int min=0;
int sec=0;
int start=0;
int check=1;

void beep() {
  lcd.noBacklight();
  digitalWrite(7, HIGH);
  delay(300);
  lcd.backlight();
  digitalWrite(7, LOW);
  delay(200);
}

void showtime(){
  if(hour>=10){
    lcd.setCursor(1,1);
  }
  else{
    lcd.setCursor(1,1);
    lcd.print(" ");
    lcd.setCursor(2,1);
  }
  lcd.print(hour);
  lcd.setCursor(4,1);
  lcd.print("h");
  if(min>=10){
    lcd.setCursor(6,1);
  }
  else{
    lcd.setCursor(6,1);
    lcd.print(" ");
    lcd.setCursor(7,1);
  }
  lcd.print(min);
  lcd.setCursor(9,1);
  lcd.print("m");
  if(sec>=10){
    lcd.setCursor(11,1);
  }
  else{
    lcd.setCursor(11,1);
    lcd.print(" ");
    lcd.setCursor(12,1);
  }
  lcd.print(sec);
  lcd.setCursor(14,1);
  lcd.print("s");
}

void setup(){
  pinMode(13, INPUT);
  pinMode(12, INPUT);
  pinMode(11, INPUT);
  pinMode(7, OUTPUT);
  pinMode(8, INPUT);
  lcd.init();
  lcd.backlight();
  lcd.setCursor(3, 0);
  lcd.print("Alarm Clock ");
  delay(3000);
  lcd.clear();
  lcd.setCursor(0, 0);
  lcd.print("Please set time");
}

void loop(){
  int sound=0;
  
  delay(500);
  lcd.clear();
  lcd.setCursor(0, 0);
  lcd.print("Set hour");
  while(1){
    if(digitalRead(11) == LOW){
      break;
    }
    if(digitalRead(13)== LOW){
      hour++;
    }
    else if(digitalRead(12)== LOW){
      hour--;
    }
    if (hour < 0){
      hour = 0;
    }
      delay(100);
      lcd.setCursor(10,0);
      lcd.print(hour);
      lcd.print(" h ");
      showtime();
  }
  
  delay(500);
  lcd.clear();
  lcd.setCursor(0, 0);
  lcd.print("Set minute");
  while(1){
    if(digitalRead(11) == LOW){
      break;
    }
    if(digitalRead(13)== LOW){
      min++;
    }
    else if(digitalRead(12)== LOW){
      min--;
    }
    if (min < 0){
      min = 59;
    }
    if (min >= 60){
      min = 0;
    }
      delay(100);
      lcd.setCursor(12,0);
      lcd.print(min);
      lcd.print(" m ");
      showtime();
  }
  
  delay(500);
  lcd.clear();
  lcd.setCursor(0, 0);
  lcd.print("Set second");
  while(1){
    if(digitalRead(11) == LOW || digitalRead(8) == LOW){
      break;
    }
    if(digitalRead(13)== LOW){
      sec++;
    }
    else if(digitalRead(12)== LOW){
      sec--;
    }
    if (sec < 0){
      sec = 59;
    }
    if (sec >= 60){
      sec = 0;
    }
      delay(100);
      lcd.setCursor(12,0);
      lcd.print(sec);
      lcd.print(" s ");
      showtime();
  }
  
  lcd.clear();
  delay(200);
  lcd.setCursor(2,0);
  lcd.print(hour);
  lcd.print(" h ");
  lcd.print(min);
  lcd.print(" m ");
  lcd.print(sec);
  lcd.print(" s ");
  lcd.setCursor(4,1);
  lcd.print("Started !");
  delay(1000);
  lcd.clear();
  start=1;
  int msec = 52.5;
  int status = 1;
  while(1){
    if (status == 0){
      if (digitalRead(11) == LOW && status == 0){
        status = 1;
        delay(500);
        lcd.clear();
      }
    }
    else if(digitalRead(11) == LOW && status == 1){
      status = 0;
      lcd.setCursor(0,1);
      lcd.print("Stoped!!");
      delay(500);
    }
    if(status == 1){
      if (msec == 0){
        sec--;
        msec = 52.5;
      }
      if(hour==0 && min==0 && sec==0){
        start=1;
        break;
      }
      if(min!=0 && sec == -1){
        min--;
        sec=59;
      }
      if(hour!=0 && min==0 && sec==-1){
        hour--;
        min=59;
        sec=59;
      }
      msec--;
    }
    lcd.setCursor(2,0);
    lcd.print(hour);
    lcd.print(" h ");
    lcd.print(min);
    lcd.print(" m ");
    lcd.print(sec);
    lcd.print(" s ");
  }
  lcd.clear();
  delay(200);
  lcd.setCursor(2,0);
  lcd.print(hour);
  lcd.print(" h ");
  lcd.print(min);
  lcd.print(" m ");
  lcd.print(sec);
  lcd.print(" s ");
  lcd.setCursor(4,1);
  lcd.print("Alert !");
  while(sound<3){
    beep();
    sound++;
  }
  while(digitalRead(11) != LOW){}
  hour=0;
  min=0;
  sec=0;
  start=0;
}
