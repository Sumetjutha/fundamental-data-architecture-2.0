# Fundamental Course of Data Architecture 2.0 (101 Level)

## สรุปเนื้อหาเป็นภาษาไทย

คอร์สนี้เป็นคอร์สพื้นฐานระดับ 101 สำหรับทำความเข้าใจ **Data Architecture** หรือ “สถาปัตยกรรมข้อมูล” ซึ่งเป็นแนวคิดสำคัญในการออกแบบว่าองค์กรจะเก็บ ใช้ จัดการ เชื่อมโยง และควบคุมข้อมูลอย่างไรให้เป็นระบบ

---

## 1. Data Architecture คืออะไร

**Data Architecture** คือชุดของกฎ นโยบาย มาตรฐาน โมเดล และแนวทางการออกแบบข้อมูลในองค์กร โดยกำหนดว่า

- องค์กรควรเก็บข้อมูลประเภทใด
- ข้อมูลถูกนำไปใช้อย่างไร
- ข้อมูลถูกจัดเก็บไว้ที่ไหน
- ข้อมูลถูกจัดการและเชื่อมโยงระหว่างระบบอย่างไร
- ระบบ IT และ Application ต่าง ๆ สร้างและส่งผ่านข้อมูลกันอย่างไร

พูดง่าย ๆ คือ Data Architecture เป็น “พิมพ์เขียวของข้อมูล” ที่ทำให้ข้อมูลในองค์กรไม่กระจัดกระจาย และสามารถนำไปใช้งานต่อได้อย่างมีประสิทธิภาพ

---

## 2. ทำไม Data Architecture ถึงสำคัญ

Data Architecture สำคัญเพราะช่วยให้องค์กร

- เข้าใจข้อมูลของตัวเองมากขึ้น
- รู้ว่าข้อมูลมาจากไหน
- รู้ว่าข้อมูลถูกจัดเก็บและใช้งานอย่างไร
- จัดการข้อมูลตั้งแต่เริ่มเก็บจนถึงนำไปใช้วิเคราะห์ได้เป็นระบบ
- ลดความซ้ำซ้อนและความสับสนของข้อมูล
- สนับสนุนการทำ Data Warehouse, Business Intelligence, Data Governance และ Analytics

ถ้าองค์กรไม่มี Data Architecture ที่ดี ข้อมูลอาจกระจัดกระจาย ซ้ำซ้อน คุณภาพต่ำ และยากต่อการนำไปใช้ตัดสินใจทางธุรกิจ

---

## 3. บทบาทของ Data Architect

Data Architect คือคนที่ออกแบบ สร้าง วางระบบ และดูแลภาพรวมของโครงสร้างข้อมูลในองค์กร

หน้าที่หลัก เช่น

- ออกแบบโครงสร้างข้อมูล
- กำหนดมาตรฐานข้อมูล
- วางแนวทางการเชื่อมโยงข้อมูลระหว่างระบบ
- ออกแบบ Data Model
- ทำงานร่วมกับทีม Business, Data Engineer, BI Developer, DBA และ IT
- ช่วยให้องค์กรใช้ข้อมูลได้อย่างถูกต้อง ปลอดภัย และมีประสิทธิภาพ

---

## 4. 3 Layers ของ Enterprise Data Architecture

Data Architecture ในระดับองค์กรสามารถแบ่งออกเป็น 3 ชั้นหลัก

### 4.1 Conceptual / Business Model

เป็นระดับภาพรวมทางธุรกิจ

เน้นตอบคำถามว่า

- องค์กรมีข้อมูลสำคัญอะไรบ้าง
- Entity หลัก ๆ คืออะไร เช่น Customer, Product, Order, Payment
- ข้อมูลแต่ละกลุ่มมีความหมายทางธุรกิจอย่างไร

ชั้นนี้ช่วยให้ Business และ IT เข้าใจตรงกัน

---

### 4.2 Logical / System Model

เป็นระดับที่อธิบายความสัมพันธ์ของข้อมูล

เน้นตอบคำถามว่า

- Entity ต่าง ๆ เชื่อมโยงกันอย่างไร
- Customer เกี่ยวข้องกับ Order อย่างไร
- Product เกี่ยวข้องกับ Transaction อย่างไร
- ข้อมูลควรมี Attribute อะไรบ้าง

ชั้นนี้ยังไม่ผูกกับ Technology มากนัก แต่เริ่มลงรายละเอียดเชิงระบบมากขึ้น

---

### 4.3 Physical / Technology Model

เป็นระดับที่นำแบบจำลองข้อมูลไปสร้างจริงบน Technology

เน้นตอบคำถามว่า

- ใช้ Database อะไร
- Table หน้าตาอย่างไร
- Column มี Data Type อะไร
- Index, Partition, Storage และ Performance ต้องออกแบบอย่างไร
- ระบบจะ Deploy บน Infrastructure แบบไหน

ชั้นนี้ใกล้กับงานของ DBA, Data Engineer และ System Engineer มากที่สุด

---

## 5. หัวข้อหลักของคอร์ส

คอร์สนี้แบ่งเนื้อหาออกเป็น 5 หัวข้อหลัก

### 5.1 Data Architecture 2.0 คืออะไร และทำไมจึงเกี่ยวข้อง

อธิบายภาพรวมของ Data Architecture ยุคใหม่ ว่ามีบทบาทอย่างไรกับองค์กรที่ใช้ข้อมูลในการตัดสินใจ

---

### 5.2 ประเภท ชั้น Framework และ DBMS

อธิบายประเภทของ Data Architecture, Layer ต่าง ๆ, Framework ที่เกี่ยวข้อง และระบบจัดการฐานข้อมูล เช่น DBMS

---

### 5.3 Function, Principle และ Pattern ของ Data Architecture 2.0

อธิบายหน้าที่ หลักการ และรูปแบบการออกแบบ Data Architecture ที่ใช้ซ้ำได้ในองค์กร

---

### 5.4 Data Architecture สำหรับ Business และ Business Intelligence

เชื่อมโยง Data Architecture กับการใช้งานทางธุรกิจ เช่น Reporting, Dashboard, BI และ Decision Making

---

### 5.5 Career Path และ Skills ของ Data Architect

อธิบายเส้นทางอาชีพและทักษะที่จำเป็นสำหรับคนที่อยากเป็น Data Architect เช่น

- Data Modeling
- Database Design
- Data Governance
- Data Integration
- Business Understanding
- Cloud / Infrastructure
- Communication Skill

---

## 6. สรุปแบบเข้าใจง่าย

Data Architecture คือการออกแบบ “ระบบนิเวศของข้อมูล” ในองค์กร ตั้งแต่ว่าข้อมูลคืออะไร อยู่ที่ไหน ไหลไปไหน ใครใช้ และต้องดูแลอย่างไร

สำหรับคนสาย Data Engineer หรือ Data Warehouse ความรู้นี้สำคัญมาก เพราะช่วยให้เราไม่ได้มองแค่การเขียน ETL หรือ Query แต่เริ่มมองภาพใหญ่ของระบบข้อมูลทั้งองค์กร

---

## 7. Key Takeaways

- Data Architecture คือพิมพ์เขียวของข้อมูลในองค์กร
- ช่วยจัดระเบียบการเก็บ ใช้ จัดการ และเชื่อมโยงข้อมูล
- มี 3 ระดับหลัก: Conceptual, Logical, Physical
- Data Architect ต้องเข้าใจทั้ง Business, Data Model, Database และ Technology
- ความรู้นี้เป็นพื้นฐานสำคัญก่อนขยับไปสู่ Data Architect, Analytics Engineer หรือ Data Platform Lead

---

## 8. Note สำหรับการเรียนต่อ

หลังจากเรียนหัวข้อนี้ ควรต่อยอดด้วยหัวข้อเหล่านี้

1. Data Modeling
2. Data Warehouse Architecture
3. Dimensional Modeling
4. Data Governance
5. Data Integration
6. Cloud Data Platform
7. Business Intelligence Architecture
