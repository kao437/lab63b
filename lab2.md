# การทดลองที่2 การเขียนโปรเเกรมเพื่อค้นหาไวไฟ
## วัตถุประสงค์ 
1. เพื่อศึกษาการค้นหา wifi ที่อยู่รอบๆ ของไมโครคอนโทลเลอร์

## อุปกรณ์ที่ใช้
1. microcontroller ESP01
2. อุปกรณ์ต่อ USB

## ศึกษาข้อมูลเบื้องต้น
run example 2 : https://www.youtube.com/watch?v=yBjab0UNuB8
code 02_Scan-WIFI : https://github.com/choompol-boonmee/lab63b/blob/master/examples/02_Scan-Wifi/platformio.ini

## วิธีการทดลอง
1. นำไมโครคอนโทลเลอร์ เข้ากับอุปกรณ์ต่อ USB
2. เตรียมที่จะอัพโหลดโปรแกรมเข้าด้วยคำสั่ง vi src/main.cpp
3. อัพโหลดโปรแกรมเข้าสู่ไมโครคอลโทลเลอร์ด้วยคำสั่ง pio run -t upload
4. เมื่ออัพโหลดเสร็จจะพิมพ์คำสั่ง pio device monitor เพื่อดูว่าเจอWIFIอะไรบ้าง
![image](https://user-images.githubusercontent.com/80883602/112296896-d5e70600-8cc7-11eb-93b7-6a2f1e8b42ce.png)

## การบันทึกผลการทดลอง
เมื่อเราพิมพ์คำสั่ง  pio device monitor ไมโครคอนโทลเลอร์จะเริ่มสแกนหาWIFIที่ตรวจพบ

## อภิปรายผลการทดลอง
จากการทดลองการเขียนโปรแกรมเพื่อค้นหาไวไฟ จะเห็นว่าหลังจากเราทำการอัพโหลดโปรแกรมลงบนไมโครคอนโทลเลอร์ และพิมพ์คำสั่ง pio device monitor แล้วหน้าจอจะเเสดง WIFIที่รวจพบตามลำดับความแรงของสัญญาณ

## คำถามหลังการทดลอง
ไมโครคอนโทลเลอร์จะสามารถรับ WIFI ได้เเละรันขึ้นมาได้เร็วจาก
ตอบความเเรงของสัญญาญ
