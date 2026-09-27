# แปลงคำตอบ Google Form เป็น PDF

เว็บแอปไฟล์เดียว (`index.html`) ใช้แปลงไฟล์ผลลัพธ์ Google Form (.csv / .xlsx) เป็น PDF
ข้อมูลทั้งหมดประมวลผลบนเครื่องผู้ใช้ ไม่มีการส่งขึ้นเซิร์ฟเวอร์

## ขั้นตอนอัปขึ้น GitHub Pages

1. เข้า https://github.com แล้วล็อกอิน
2. กด **New repository** ตั้งชื่อ เช่น `form-to-pdf` เลือก **Public** แล้วกด **Create repository**
3. ในหน้า repo กด **uploading an existing file** (หรือ Add file › Upload files)
4. ลาก `index.html` และ `README.md` มาวาง แล้วกด **Commit changes**
5. ไปที่ **Settings › Pages**
   - Source: **Deploy from a branch**
   - Branch: **main** / **(root)** แล้วกด **Save**
6. รอ 1–2 นาที แล้วรีเฟรชหน้า Settings › Pages จะเห็นลิงก์
   `https://<ชื่อผู้ใช้>.github.io/form-to-pdf/`

## อัปเดตเวอร์ชันใหม่
เข้า repo › Add file › Upload files › วาง `index.html` ไฟล์ใหม่ทับ › Commit changes

## หมายเหตุ
- ต้องต่ออินเทอร์เน็ต เพราะฟอนต์และไลบรารีสร้าง PDF / อ่าน Excel / ZIP โหลดจาก CDN
- repo แบบ Public ใครก็เห็นโค้ดได้ แต่ไม่เห็นข้อมูลที่ผู้ใช้อัปโหลด (ข้อมูลอยู่บนเครื่องผู้ใช้เท่านั้น)
- ไฟล์ Private repo ใช้ GitHub Pages ได้เฉพาะบัญชีแบบเสียเงิน
