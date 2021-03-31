# การทดลองที่ 7 เรื่อง ควบคุมเปิดปิดไฟบ้านด้วย web server
## วัตถุประสงค์
1. เพื่อลองศึกษษการเขียนโค้ดในรูปแบบต่างๆ
2. เพื่อให้นำความรู้ตั้งแต่การทดลองที่ 1-6 มาประยุกต์
## อุปกรณ์ที่ใช้
1. microcontroller
2. อุปกรณ์เชื่อมต่อ USB 
3. โทรศัพท์มือถือเพื่อเข้า web server
4. หลอด LED
## ศึกษาข้อมูลเบื้องต้น
1. 01 run example 1 : https://www.youtube.com/watch?v=NLIUsWLEpmg
2. 02 run example 2 : https://www.youtube.com/watch?v=yBjab0UNuB8
3. 03 run example 3 : https://www.youtube.com/watch?v=CCnN1WJsXQY
4. 04 run example 4 : https://www.youtube.com/watch?v=nFqoZT26U5k&t=13s
5. 05 run wifi : https://www.youtube.com/watch?v=VX-QNQcO-b4&t=226s
6. 06 run wiri AP : https://www.youtube.com/watch?v=T26DVHePlTs
7. code : https://github.com/choompol-boonmee/lab63b/tree/master/examples
## วิธีทำการทดลอง
1. ต่ออแดปเตอร์เข้ากับอุปกรณ์เชื่อต่อUSB
2. นำไมโครคอลโทลเลอร์เข้ากับอแดปเตอร์
3. พิมพ์คำสั่ง cd 07_ligth-web แล้วพิมพ์คำสั่ง vi src/main.cpp 
![image](https://user-images.githubusercontent.com/80883602/113205967-1121a000-9299-11eb-8cb3-0bcf79580355.png)
![image](https://user-images.githubusercontent.com/80883602/113205985-167eea80-9299-11eb-9f77-95d8898219e3.png)
4. อัพโหลดโปรแกรมเข้าไมโครคอนโทลเลอร์ด้วยคำสั่ง pio run-t upload แล้วกดปุ่มรีเซ็ตเพื่อให้โปรแกรมอัพโหลด
6. พิมพ์คำสั่ง pio device monitor 
7. หลังจากนั้นเข้าไปที่หน้าเว็ป 192.168.4.1
## การบันทึกผลการทดลอง
จะเห็นว่าเราสามารถควบคุมการปิด/เปิดของไฟLEDได้ผ่านทางคอมพิวเตอร์หรือโทรศัพท์ที่เชื่อมอินเตอร์เน็ตโดยการเข้าไปใน web server เพื่อสั่งเปิด/ปิดไฟ
## อภิปรายผลการทดลอง
เนื่องจากช่วงนี้มีการแพร่ระบาดของโรค COVID 19 ทำให้ไม่สามารถทำการทดสอบว่าโค้ดที่เราเขียนนั้นถูกหรือไม่ แต่ด้วยความรู้จากทั้ง6การทดลองทำให้ประยุกต์ออกมาเป็นการทดลองที่ 7
## คำถามหลังการทดลอง
เราสามารถเพิ่มจำนวนหลอดไฟที่เราควบคุมได้หรือไม่ ตอบได้
