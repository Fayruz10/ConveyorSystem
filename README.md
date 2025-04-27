# Industrial Automation : Sorting System Based on color For efficiency in Industrial Automation

---

## Mata Kuliah
*Pemrograman Kontroller* 
Dosen Pengampu: Ahmad Radhy, S.Si., M.Si

---

## Anggota Kelompok

1. Dina Nur Shadrina / 2042231026
2. Muhammad Fayruz Zamzamy / 2042231032
3. Raditya Wahyu Prasetyo / 2042231034



---

## Fungsi Alat
- Mengembangkan program yang mampu membaca data sensor, memproses keputusan sortir, serta mengendalikan aktuator dan indikator sistem secara otomatis dan real-time.
- Menyusun sistem program yang mengintegrasikan seluruh komponen kendali dan monitoring secara modular agar memudahkan dalam proses pengujian dan pengembangan lebih lanjut.
- Melakukan unit testing terhadap bagian-bagian program menggunakan Programiz sebagai alat bantu pengujian, untuk memastikan setiap bagian kode berjalan sesuai dengan fungsinya dan memenuhi prinsip keandalan sistem kendali. 

---

## Komponen yang digunakan
- Sensor Warna TCS34725
- Motor Servo Delta ECMA-C20604RS
- Motor Stepper NEMA 34
- PWM (Pulse Width Modulation)
- Buzzer
  
---

## 🚀 Cara Menggunakan

1. *Clone repository*
   ```bash
   git clone https://github.com/nazwana/AgroBot.git

---


## 📚 Tutorial Setup Program Robot
- Pada halaman awal pilih Start my project from ST Board.  
  ![](DOKUMENTASI_CONTROLLER/Screenshot%20(43).png)
- Pada bagian comercial part number pilih STM32F446RE dan klik Strart Project.  
  ![](DOKUMENTASI_ROBOT/Screenshot%20(56).png)
- Pada System Core klik Sys, atur debug ke Serial Wire  
  ![](DOKUMENTASI_ROBOT/Screenshot%20(45).png)
- Pada bagian RCC, atur High Speed Clock(HSE) dan Low Speed Clock (LSE) Crystal/Ceramic Resonator  
  ![](DOKUMENTASI_ROBOT/Screenshot%20(46).png)
- Pada GPIO, atur PA5 dan PC3 sebagai GPIO Output.  
  ![](DOKUMENTASI_ROBOT/Screenshot%20(47).png)
- Pada ANALOG, aktifkan ADC3 channel IN12. Pada Parameter Settings aktifkan Contonous Conversion Mode.   
  ![](DOKUMENTASI_ROBOT/Screenshot%20(48).png)
- Pada TIMER, aktifkan TIM2 CH1 untuk Servo, TIM3 CH1 untuk DHT11, TIM10 CH1 untuk motor 1, TIM11 CH1 untuk motor 2, TIM12 CH1 untuk motor 3 dan CH2 untuk motor 4.
  ![](DOKUMENTASI_ROBOT/Screenshot%20(49).png)
  ![](DOKUMENTASI_ROBOT/Screenshot%20(50).png)
  ![](DOKUMENTASI_ROBOT/Screenshot%20(51).png)
  ![](DOKUMENTASI_ROBOT/Screenshot%20(52).png)
- Pada Conectivity, aktifkan SPI1 dan atur ke Full Duplex Slave dan aktifkan USART2 Asynchronus Mode.
  ![](DOKUMENTASI_Robot/Screenshot%20(53).png) 
  ![](DOKUMENTASI_Robot/Screenshot%20(54).png)
- Pada Clock Configuration tidak perlu diubah dan biarkan secara default.   
  ![](DOKUMENTASI_Robot/Screenshot%20(55).png)
- Pada Project Manager, Beri nama project dan atur Toolchain jadi MDK ARM, kemudian klik generate code.   
  ![](DOKUMENTASI_ROBOT/Screenshot%20(57).png)
- Setelah itu edit program pada main.c

---

## 📚 Tutorial Setup Program Controller
- Pada halaman awal pilih Start my project from MCU.  
  ![](DOKUMENTASI_CONTROLLER/Screenshot%20(43).png)
- Pada bagian comercial part number pilih STM32F103C8T6 dan klik Strart Project.  
  ![](DOKUMENTASI_CONTROLLER/Screenshot%20(44).png)
- Pada System Core klik Sys, atur debug ke Serial Wire  
  ![](DOKUMENTASI_CONTROLLER/Screenshot%20(24).png)
- Pada bagian RCC, atur High Speed Clock(HSE) Crystal/Ceramic Resonator  
  ![](DOKUMENTASI_CONTROLLER/Screenshot%20(25).png)
- Pada bagian IWDG, klik activated dan atur prescaler dengan nilai 32 dan IWDG counter value 4095.  
  ![](DOKUMENTASI_CONTROLLER/Screenshot%20(26).png)
- Pada GPIO, atur PA4,PB12,PB13,PB14,PB15 sebagai GPIO Output dan PB3 PB4 sebagai GPIO Input.  
  ![](DOKUMENTASI_CONTROLLER/Screenshot%20(27).png)
- Pada ANALOG, aktifkan ADC1 channel IN0 dan IN1. Pada Parameter Settings aktifkan Contonous Conversion Mode.   
  ![](DOKUMENTASI_CONTROLLER/Screenshot%20(28).png)
- Pada Conectivity, aktifkan SPI1 dan atur ke Full Duplex Master dan atur presclaer baud rate ke 16.   
  ![](DOKUMENTASI_CONTROLLER/Screenshot%20(30).png)
- Pada Clock Configuration, atur ke HSE dan ubah HCLK jadi 72MHz.   
  ![](DOKUMENTASI_CONTROLLER/Screenshot%20(31).png)
- Pada Project Manager, Beri nama project dan atur Toolchain jadi MDK ARM, kemudian klik generate code.   
  ![](DOKUMENTASI_CONTROLLER/Screenshot%20(33).png)
- Setelah terbuka Keil, klik kanan Aplication/User/Core dan masukkan library NRF2L401.c yang telah dibuat.   
  ![](DOKUMENTASI_CONTROLLER/Screenshot%20(34).png)
- Pada option for target, atur ARM Compiler menjadi Use Default Compiler Version 6.   
  ![](DOKUMENTASI_CONTROLLER/Screenshot%20(35).png)
- Setelah itu edit program pada main.c
  
---

## 🖼 Dokumentasi dan Demo
Link PPT : (https://its.id/m/PPTAGROBOT).

---

## 📌 Saran untuk Pengembangan Selanjutnya
- Integrasi dengan IoT dashboard untuk monitoring dari jarak jauh
- Penambahan AI untuk klasifikasi penyakit tanaman
- Manajemen energi dengan panel surya

---
