# การทดลองที่1 เรื่องการเขียนโปรแกรมเพื่อรันบนไมโครคอนโทลเลอร์
## วัตถุประสงค์
1. เพื่อศึกษาการใช้งานคำสั่งต่างๆ ที่จะรันโปรแกรม
2. เพื่อศึกษาข้อมูลพื้นฐานของไมโครคอนโทลเลอร์ที่ใช้ในการรันโปรเเกรม
3. เพื่อศึกษาการเขียนโปรแกรมเพื่อรันบนไมโครคอนโทลเลอร์
## อุปกรณ์ที่ใช้
1. ไมโครคอนโทลเลอร์
2. อุปกรณ์ USB
3. CPU
## ศึกษาข้อมูลเบื้องต้น
1. 01 run example 1 : https://www.youtube.com/watch?v=NLIUsWLEpmg
2. code 01_Serial-Monitor: https://github.com/choompol-boonmee/lab63b/blob/master/examples/01_Serial-Monitor/src/main.cpp
3. plaformio : https://platformio.org/
## วิธีทำการทดลอง
1. ต่อไมโครคอนโทลเลอร์กับซีเรียล
2. เข้าcommand prompt แล้วพิมคำสั่ง cd pattani เพื่อเข้าโปรแกรมตัวอย่าง cd 01_Serial-Monitor
3. พิมคำสั่ง vi src/main.cpp 
![image](https://user-images.githubusercontent.com/80883602/112285674-260c9b00-8cbd-11eb-9878-5c38f94982d6.png)

4.พิมพ์คำสั่ง vi platformio.ini 
![image](https://user-images.githubusercontent.com/80883602/112363140-bff93580-8d07-11eb-8309-17b260366f3d.png)

5. ทำการอัพโหลดโปรแกรม01 serial เข้าไมโครคอนโทลเลอร์ด้วยคำสั่ง pio run -t upload 
![image](https://user-images.githubusercontent.com/80883602/112288245-ba77fd00-8cbf-11eb-820d-8874b030f167.png)

6. กดปุ่มรีเซ็ตแล้ว พิมพ์คำสั่งpio device monitor เพื่อดูผลลัพท์
![image](https://user-images.githubusercontent.com/80883602/112288793-4853e800-8cc0-11eb-9484-61c8961a1d45.png)

## บันทึกผลการทดลอง
คำสั่ง pio device monitor จะเป็นการเพิ่มค่าตัวแปร countขึ้นทุกๆ1วินาที และเมื่อกดรีเซ็ตจะนับ1ใหม่อีกครั้ง
## อภิปรายการทดลอง
จากการใช้คำสั่ง vi src/main.cpp ทำให้เราทราบว่าโปรแกรม 01_Serial-Monitor มี2 ส่วน ดังนี้
ส่วน set up ซึ่งจะรันแค่รอบเดียว และ ส่วน loop ในส่วนของloopนั้นคือการแสดง ตัวแปรcount และมีค่าเพิ่มขึ้นที่ละ1 ซึ่งจะรันวนไปเรื่อยๆ
## คำถามหลังการทดลอง
ถ้าเราอยากรู้ว่าเป็นplatformของบริษัทไหนต้องพิมพ์คำสั่งอะไร ตอบ vi platformio.ini
