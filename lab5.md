# การทดลองที่ 5 การเขียนโปรแกรมเชื่อมต่อWIFIและเว็ปเซิร์ฟเวอร์
## จุดประสงค์
1. เพื่อศึกษาการเขียนโปรแกรมเพื่อเชื่อมต่อWIFIและเว็ปเซิร์ฟเวอร์
## อุปกรณ์ที่ใช้
1. ไมโครคอนโทลเลอร์
2. อุปกรณ์ต่อ USB 
3. ตัวโปรแกรมเชื่อมต่อไวไฟและเซิร์ฟเวอร์
## ศึกษาข้อมูลเบื้องต้น
05 run wifi : https://www.youtube.com/watch?v=VX-QNQcO-b4&t=19s
code 05_run_wifi : https://github.com/choompol-boonmee/lab63b/blob/master/examples/05_Wifi-Web-Server/src/main.c
## วิธ๊ทำการทดลอง
1. ใช้คำสั่ง cd pattani ตามด้วย 05_run_wifi ตามด้วยคำสั่ง 1s จากนั้นพิมคำสั่ง vi src/main.cpp![image](https://user-images.githubusercontent.com/80883602/112357565-3c891580-8d02-11eb-94e8-3c27722476e6.png)

2. setup เป็น connectกับ wifi ที่เราใส่ชื่อไวในตอนแรก และsetup เซิร์ฟเวอร์ โดยการเเสดงผล Hello cnt โดยที่cnt จะมีค่าเพิ่มขึ้นทีละ1 ไปเลื่อยๆ
3. ต่อไมโครคอนโทลเลอร์เข้ากับอุปกรณ์ต่อ USB
4. อัพโหลดโปรแกรมเข้าไปในไมโครคอนโทลเลอร์ 
5. พิมพ์คำสั่ง pio device monitor ![image](https://user-images.githubusercontent.com/80883602/112357767-693d2d00-8d02-11eb-9328-c26fbf172bb6.png)

## การบันทึกการทดลอง
เมื่อทำการพิมพ์คำสั่ง pio device monitor ไมโครคอนโทลเลอร์จะทำการแสดง ip address จากนั้นคัดลอก ip address ไปที่browserหน้าเจอก็เจอแสดง Hello 1 เพิ่มขึ้นที่ละ1ไปเลื่อย
## อภิปรายการทดลอง
จากการทดลองสามารถสรุปได้ว่าไมโครคอนโทลเลอร์สามารถเชื่อมต่อWIFIและเว็ปเซิร์ฟเวอร์ และทำงานได้เหมือนเว็ปเซิร์ฟเวอร์อื่นๆ
## คำถามหลังการทดลอง
การที่หน้าจอแสดงผล Hello 1 และเพิ่มขึ้นที่ละ1มาจากส่วนไหนของโปรแกรม ตอบมากจาก loop
