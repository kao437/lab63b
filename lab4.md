# การทดลองที่ 4 การเขียนโปรแกรมอินพุทสัญญาณดิจิทัล
## วัตถุประสงค์
1. เพื่อศึกษาการเขียนโปรแกรมอินพุทของสัญญาณดิจิตัล
## อุปกรณ์ที่ใช้
1. ไมโครคอนโทลเลอร์
2. อแดปเตอร์
3. หลอดไฟ LED
4. อุปกรณ์ต่อ USB
5. ตัวเซนเซอร์แสง
6. ตัวโปรแกรมเอาท์พุตสัญญาณ
## ศึกษาข้อมูลเบื้องต้น
1. 04 run example 4 : https://www.youtube.com/watch?v=nFqoZT26U5k&t=12s
2. code ของโปรแกรม 04_input-Port : https://github.com/choompol-boonmee/lab63b/blob/master/examples/04_Input-Port/src/main.cpp
## วิธีทำการทดลอง
1. นำอแดปเตอร์ต่อกับอุปกรณ์ต่อ USB 
2. นำไมโครคอนโทลเลอร์
3. เข้า command prompt จากนั้นพิมพ์ cd pattani แล้วเลือกตัวอย่างโปรแกรมคำสั่ง cd 04_input-Port ตามคำสั่ง 1s และ pwd
4. พิมพ์ vi src/main.cpp 
![image](https://user-images.githubusercontent.com/80883602/112347912-e0ba8e80-8cf9-11eb-990d-a4f11289bc3a.png)
5. อัพโหลดโปรแกรมเข้าไปในไมโครคอนโทลเลอร์ และกดปุ่มรีเซ็ต
6. พิมพ์คำสั่ง pio device monitor
7. จากนั้นลองนำสายสีขาว (พอร์ท 0) จิ้มเข้ากับเส้นสีดำ 
![image](https://user-images.githubusercontent.com/80883602/112349653-7e628d80-8cfb-11eb-925f-6c6a510dcb98.png)

8. นำสายสีขาว (พอร์ท 0) จิ้มเข้ากับเส้นแดง
![image](https://user-images.githubusercontent.com/80883602/112349679-83274180-8cfb-11eb-9c71-b3d145f3dc42.png)

9. เมื่อกดปุ่มสีดำ (พอร์ท 0=0) input=0
![image](https://user-images.githubusercontent.com/80883602/112352808-aeab2b80-8cfd-11eb-8bf3-adb36157044d.png)
10. เมื่อปล่อย input=1
![image](https://user-images.githubusercontent.com/80883602/112352788-a94de100-8cfd-11eb-934d-61b54509f8a7.png)
11. นำเซนแสงต่อเข้าดังรูป
![image](https://user-images.githubusercontent.com/80883602/112352246-32184d00-8cfd-11eb-8ac0-6297c9d73207.png) 
12. เอานิ้วไปบังหน้าเซนเซอร์ ![image](https://user-images.githubusercontent.com/80883602/112352858-bb2f8400-8cfd-11eb-975c-9d89675d91cc.png)

13. เอานิ้วออกหน้าเซนเซอร์
![image](https://user-images.githubusercontent.com/80883602/112352730-989d6b00-8cfd-11eb-88c1-b6bb4b11f606.png)
## การบันทึกผลการทดลอง
จะเหฌนว่าหลังจากเราอัพโหลดโปรแกรมและพิมพ์คำสั่ง pio devicemonitor ขึ้นว่าread1 ทำให้lowทำให้ไฟไม่ติด
เมื่อจิ้มอินพุตเข้าไปที่สีดำ input = 0  high ไฟติด
เมื่อจิ้มอินพุตเข้าไปที่สีแดง input = 1  low ไฟดับ
## อภิปรายผลการทดลอง
จากการทดลองเขียนโปรแกรมสามารถสรุปได้ว่า สัญญาณอินพุตจากพอร์ท 0 คือตัวควบคุม ให้ไฟเปิด-ปิด ถ้า 1ไฟจะติด ถ้า0 ไฟจะดับ
## คำถามหลังการทดลอง
ทำไมเมื่อเรานำมือไปปิดแล้วไฟ้ถึงดับ ตอบเพราะเมื่อมีแสงเข้ามที่เส้นเซอร์ทำให้ค่าความต้านทานเข้าใกล้0แต่เมื่อนำนิ้วมาปิดค่าความต้านทานจะมีค่ามากขึ้นทำให้ไฟดับ
