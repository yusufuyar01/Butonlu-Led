# Butonlu Led

Bu proje, Arduino kullanarak basit bir LED'i kontrol etmeyi amaçlar. LED'i Arduino'nun 8. pinine bağlayarak, basit bir kod ile LED'in yanmasını sağlamaktayız.

## Gerekli Malzemeler

*   Arduino Geliştirme Kartı
*   1 adet LED
*   1 adet 220 Ohm Direnç (LED'i korumak için)
*   Jumper Kabloları
*   Breadboard (isteğe bağlı)

## Bağlantı Şeması

1.  LED'in uzun bacağını (anot) Arduino'nun 8. pinine bağlayın.
2.  LED'in kısa bacağını (katot) 220 Ohm direnç üzerinden Arduino'nun GND (toprak) pinine bağlayın.  
  ![Image](https://github.com/user-attachments/assets/355d39ef-80ea-4528-9a3f-10128ec53b99)

## Kod

```c++
int led = 8; // LED'in bağlı olduğu pin

void setup() {
  pinMode(led, OUTPUT); // 8. pini çıkış olarak ayarla
}

void loop() {
  digitalWrite(led, HIGH); // LED'i yak
  // delay(1000); // 1 saniye bekle (isteğe bağlı)
  // digitalWrite(led, LOW); // LED'i söndür (isteğe bağlı)
}
 
## Kullanım
Arduino kartınızı bilgisayara bağlayın.
Arduino IDE'sini açın ve kodu yükleyin.
LED'in yandığını göreceksiniz.