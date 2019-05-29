# [NEXPIE] Backend Developer Test (ใช้ Tools อะไรก็ได้)

## เกณฑ์น้ำหนักการให้คะแนน เรียงจากมาก ไปน้อย
1. ความสมบูรณ์ และความถูกต้องของระบบ
2. คุณภาพ Code
3. Unit Testing
4. Development Document
* README
* Comment เพื่ออธิบาย Code
* API Document (*Bonus Point)
* ER Diagram (*Optional)
* Class Diagram (*Optional)
5. Dockerfile

---

## จงเขียน API และระบบดังต่อไปนี้
1. OAuth2 ใช้เพื่อขอสิทธิ์เข้าใช้งานระบบ
2. Token Management ใช้เพื่อเก็บข้อมูล Token
3. Identity and Access Management (IAM) ใช้กำหนดสิทธิ์ผู้ใช้เพื่อควบคุมเข้าถึง Resource

Note: จากระบบ NEXPIE นั้นจะมี User อยู่ 2 ชนิด คือ <br>
* User ที่เป็น Production (คนที่นำ NEXPIE ไปสร้าง Product)
* Customer เป็น End-User คือคนที่ใช้ Product

## โจทย์
1. จงออกแบบสิทธิ์การเข้าถึง NEXPIE ทั้ง User <br>
โดยปกติ User จะมีสิทธิ์ในการสร้างโปรเจค, กลุ่มของอุปกรณ์และอุปกรณ์<br>
ซึ่งในโปรเจคหนึ่ง สามารถมีได้หลาย User ที่ช่วยกันร่วม Production<br>
แต่ในแต่ละ User มีระดับสิทธิ์ที่แตกต่างกัน เช่น <br>
- สามารถลบโปรเจคได้หรือไม่ได้ 
- สามารถสร้าง/ลบกลุ่มของอุปกรณ์ได้หรือไม่ได้
- สามารถสร้าง/ลบอุปกรณ์ได้หรือไม่ได้
2. จงออกแบบสิทธิ์การเข้าถึงอุปกรณ์ของ NEXPIE ของ Customer <br>
โดย Customer จะไม่รู้ถึงการมีตัวตนเองโปรเจคและกลุ่มของอุปกรณ์ <br>
นั่นคือ Customer จะสามารถรู้จักและเข้าถึงเฉพาะอุปกรณ์ <br>
* Customer หนึ่งคนสามารถเข้าถึงได้หลายอุปกรณ์
* Customer สามารถ Add Customer คนอื่นเข้ามาใช้อุปกรณ์ของตัวเองได้
* Customer แต่ละคนจะมีสิทธิ์เข้าใช้อุปกรณ์ได้แตกต่างกัน
* อุปกรณ์สามารถอ่านและเขียนข้อมูลไปยัง NEXPIE ได้