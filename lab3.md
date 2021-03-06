# การทดลองที่ 3 การเขียนโปรแกรมเอ้าพุทสัญญาณดิจิทัล
## วัตถุประสงค์
1. เพื่อศึกษาการนำไมโครคอนโทลเลอร์ที่ถูกลงโปรแกรมแล้วไปประยุกต์ใช้
## อุปกรณ์ที่ใช้
1. ไมโครคอนโทลเลอร์
2. อุปกรณ์ต่อUSB
3. relay
4. powerbank
5. อแดปเตอร์
## ศึกษาข้อมูลเบื้องต้น
run relay : https://www.youtube.com/watch?v=6JnhaUILGuw
relay : http://www.psptech.co.th/
03_Output-Port : https://github.com/choompol-boonmee/lab63b/blob/master/examples/03_Output-Port/src/main.cpp
## วิธีทำการทดลอง
1. ต่ออแดปเตอร์เข้ากับอุปกรณ์เชื่อต่อUSB
2. นำไมโครคอลโทลเลอร์เข้ากับอแดปเตอร์
3. พิมพ์คำสั่ง cd 03_Output-Port ตามด้วยคำสั่ง 1s และคำสั่ง pwd แล้วพิมพ์คำสั่ง vi src/main.cpp 
![image](https://user-images.githubusercontent.com/80883602/112325806-94198800-8ce6-11eb-824c-83a64dff4168.png)
4. อัพโหลดโปรแกรมเข้าไมโครคอนโทลเลอร์ด้วยคำสั่ง pio run-t upload แล้วกดปุ่มรีเซ็ตเพื่อให้โปรแกรมอัพโหลด
5. พิมพ์คำสั่ง pio device monitor แล้วสังเกตุที่หลอดไฟ
![image](https://user-images.githubusercontent.com/80883602/112326291-fb373c80-8ce6-11eb-8d2d-9b43025590a3.png)
6. นำตัrelayเข้ามาต่อขับpowerbankเพื่อช่วยในการควบคุมการเปิด-ปิดของสวิตซ์
## การบันทึกผลการทดลอง
หลังจากพิมพ์คำสั่ง pio device monitorจะแสดงผล on-off สับกันไปเลื่อยๆ และport0จะไฟติดก็ต่อเมื่อ on และหลังจากที่relayควบคุมการเปิด-ปิดของสวิตซ์จะแสดงผลon-offสลับกันไปเรื่อยทุกๆ ครึ่งวินาที
## อภิปรายผลการทดลอง
จากการทดลองเมื่อไมโครคอนโทลเลอร์ถูกอัพโปรแกรม 03 Output-Port และสั่งคำสั่ง pio device monitor หน้าจอจะปรากฏ on off สลับกันทุก ครึ่งวินาที ตามโค้ดที่เราใส่ลงในโปรแกรม เเละสังเกตุหลอดไฟที่ Port 0 จะสว่างตามคำสั่งon offตามหน้าจอปรากฏและหลังนำไมโครคอนโทลเลอร์ไปใช้กับrelay ก็จะเปิดปิดสวิตซ์สอดคล้องกับคำสั่ง
## คำถามหลังการทดลอง
ทำไมถึงต้องต่อขั้วชาร์จ(powerbank)เข้ากับrelay ตอบเพราะให้กระแสไหลเข้าไปทำให้relayทำงาน

