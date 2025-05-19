# Automatic-Watering-System-With-BLYNK
Waupun gagall kasih hadiah untuk sekolah sman 2 praya dann di tolak cuman karena tidak boleh ada acara tambahan yang padahal cuman butuh 2 menit saja untuk serah terima tapi ya sudahh ndak papaa dahh lumayan lahh tambah tambah pengalaman 

## Penjelasan alatnya
jadi ini adalah projet IOT yang namanya automatic watering system yang dimana kalok bahasa indonya adalah sistem penyiram tanaman otomatis atau bisa di kontrrol melewati web atau apk android yang bernama BLYNK. jadi alat ini memiliki beberapa komponen di dalamnya yang berfungsi sebagai mendekteksi kelembapan tanah yang dimana saat tanah kering alatnya akan menyala dan sebaliknya jika tanah basah alatnya akan mati begitulah kinerja singkat dari projek ini yang disusun dan di rancang oleh Haditya Muyassar Rizki dan M. Ilham Alwan (Di tolak sekolah hadiahnya)

## Alat dan bahan 
1. esp32
2. resistive soil moisture sensor
3. relay module
4. water pump
5. 9V batre
6. lcd I2c 16x2(opsional kalau mau tampilkan statusnya)
7. kabel jumper
8. port usb

## wiringnya
## Wiring 
| Komponen                 | Pin ESP32      | Keterangan                        |
| ------------------------ | -------------- | --------------------------------- |
| **Soil Moisture Sensor** | `34 (Analog)`  | Output sensor ke pin analog ESP32 |
|                          | GND            | GND ESP32                         |
|                          | VCC            | 3.3V ESP32                        |
| **Relay Module**         | `26 (Digital)` | IN relay ke pin kontrol ESP32     |
|                          | VCC            | 5V ESP32                          |
|                          | GND            | GND ESP32                         |
|                          | NO             | Pompa air +                       |
|                          | COM            | Batre 9 Volt +                    |
| **Pompa Air**            | V+ (Power)     | NO Relay                          |
|                          | V-             | - batre 9 volt                    |
| **Batre 9 Volt**         | V-             | - batre 9 volt                    |
|                          | V+ (Power)     | COM Relay                         |
| **LCD I²C**              | SDA            | `GPIO 21 (SDA)`                   |
|                          | SCL            | `GPIO 22 (SCL)`                   |
|                          | VCC            | 5V ESP32                          |
|                          | GND            | GND ESP32                         |
