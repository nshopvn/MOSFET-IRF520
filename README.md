# MOSFET-IRF520
Mạch công suất MOSFET IRF520 được sử dụng để đóng ngắt các thiết bị công suất cao qua MOSFET IRF520 giúp bạn điều khiển các thiết bị công suất như: Motor, LED siêu sáng, quạt DC,v.v… Kích thước nhỏ, có đèn báo trạng thái hoạt động.


# Code tham khảo
int led = 9;
void setup() {
  pinMode(led, OUTPUT);
}

void loop() {
  for(int i=10;i<255;i++){
    analogWrite(9,i);
    delay(10);
  }
  for(int i=255;i>10;i--){
    analogWrite(9,i);
    delay(10);
  }
}
