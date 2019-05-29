# [NEXPIE] Backend Developer Test

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

## จงเขียนระบบดังต่อไปนี้
1. เขียน Interface สำหรับเรียกใช้ API โดยใช้ Graphql
2. OAuth2 ใช้เพื่อขอสิทธิ์เข้าใช้งานระบบ
3. Token Management ใช้เพื่อเก็บข้อมูล Token
4. Identity and Access Management (IAM) ใช้กำหนดสิทธิ์ผู้ใช้เพื่อควบคุมเข้าถึง Resource

Note: IAM ให้ใช้ Graphql เป็น Interface ในการ interactive between client และ server