# การทดลองที่ 6 การเขียนโปรแกรมสร้างWIFIแอคเซสพอยท์ (WIFI AP)
## จุดประสงค์
1.เพื่อศึกษาการเขียนโปรแกรมสำหรับไว้สร้างWIFIแอคเซสพอยท์
## อุปกรณ์ที่ใช้
1. ไมโครคอนโทลเลอร์
2. อุปกรณ์ต่อ USB 
## ศึกษาข้อมูลเบื้องต้น
06 run wiri AP : https://www.youtube.com/watch?v=T26DVHePlTs&t=65s
src code ของโปรแกรม 06_Wifi-AP-Web-Server : https://github.com/choompol-boonmee/lab63b/blob/master/examples/06_Wifi-AP-Web-Server/src/main.cpp
## วิธ๊ทำการทดลอง
1. เข้าcommand prompt จากนั้นพิมพ์คำสั่ง cd pattani เพื่อเข้าโปรแกรมตัวอย่าง cd 06_Wifi-AP-Server จากนั้นพิมพ์คำสั่ง pwd
2. พิมพ์คำสั้่ง vi src/main.cpp ![image](https://user-images.githubusercontent.com/80883602/112361141-a7881b80-8d05-11eb-98fa-18a709de9378.png)
![image](https://user-images.githubusercontent.com/80883602/112361158-ad7dfc80-8d05-11eb-8f21-cf67c5d324ca.png)
3. จากนั้นอัพโหลดโปรแกรมเข้าไมโครคอนโทลเลอร์ และกดปุ่มรีเซ็ต
4. พิมพ์คำสั่ง pio device monitor ![image](https://user-images.githubusercontent.com/80883602/112361202-b7076480-8d05-11eb-9d60-246ab3a634d4.png)
5. ทดลองใช้โทรศัพท์มือถือ หรือเครื่องมืออิเล็กโทรนิค เพื่อค้นหาWIFIที่สร้าง
## การบันทึกการทดลอง
หลังจากที่เราทำการพิมพ์คำสั่ง  pio device monitor เพื่อดูผลลัพท์ว่าWIFIที่เราสร้างได้จากการใช้เครื่องมืออิเล็กโทรนิคค้นหาชื่อWIFIที่เราสร้าง
## อภิปรายการทดลอง
เราสามารถสร้างWIFIจากไมโครคอนโทรเลอร์ได้
## คำถามหลังการทดลอง
การทดลองที่5กับการทดลองที่6ต่างกันยังไง ตอบการทดลองที่5เป็นการใช้WIFIการทดลองที่6เป็นการสร้างWIFI
