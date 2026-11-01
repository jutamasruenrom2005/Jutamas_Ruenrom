# ระบบเผยแพร่ข่าวสารและกิจกรรมของคณะวิทยาศาสตร์และวิศวกรรมศาสตร์ มก.ฉกส.

ระบบสำหรับเผยแพร่ข่าวสารและกิจกรรมของคณะวิทยาศาสตร์และวิศวกรรมศาสตร์ มหาวิทยาลัยเกษตรศาสตร์ วิทยาเขตเฉลิมพระเกียรติ จังหวัดสกลนคร โดยแบ่งการทำงานออกเป็นเว็บไซต์สำหรับผู้ใช้งานทั่วไป ระบบสำหรับผู้ดูแล และ API สำหรับจัดการข้อมูล

## 📁 Project Structure

```text
📦 KUSE Activity Management System
│
├── API-MANAGE-ACTIVITY/        # ระบบ API และฐานข้อมูล
│   ├── src/
│   │   ├── config/             # การตั้งค่าฐานข้อมูล
│   │   ├── features/           # API แยกตามฟีเจอร์
│   │   ├── middlewares/        # Middleware
│   │   ├── utils/              # ฟังก์ชันที่ใช้ร่วมกัน
│   │   ├── app.js              # ตั้งค่า Express และ API
│   │   └── server.js           # เริ่มต้นเซิร์ฟเวอร์
│   └── uploads/                # รูปภาพที่อัปโหลด
│
├── KUSE-ACTIVITY/              # เว็บไซต์สำหรับผู้ใช้งานทั่วไป
│   ├── public/images/          # รูปภาพและโลโก้
│   └── src/
│       ├── components/         # ส่วนประกอบที่ใช้ร่วมกัน
│       ├── pages/              # หน้าเว็บไซต์
│       ├── style/              # ไฟล์ CSS
│       ├── utils/              # ฟังก์ชันช่วยเหลือ
│       ├── App.jsx             # กำหนดเส้นทางเว็บไซต์
│       └── main.jsx            # จุดเริ่มต้น React
│
└── KUSE-ADMIN-ACTIVITY/        # ระบบสำหรับผู้ดูแล
    ├── public/images/          # รูปภาพและโลโก้
    └── src/
        ├── components/         # ส่วนประกอบของระบบ
        ├── modals/             # หน้าต่างเพิ่มและแก้ไขข้อมูล
        ├── pages/              # หน้าต่างต่าง ๆ ของระบบ
        ├── style/              # ไฟล์ CSS
        ├── utils/              # ฟังก์ชันและเงื่อนไขที่ใช้ร่วมกัน
        ├── App.jsx             # กำหนดเส้นทางและสิทธิ์
        └── main.jsx            # จุดเริ่มต้น React
```

## 🚀 Installation

### 1. ติดตั้ง Dependencies

เข้าไปยังโฟลเดอร์ของแต่ละโปรเจกต์และติดตั้ง Dependencies

```bash
npm install
```

### 2. เริ่มต้นใช้งานระบบ

**เว็บไซต์สำหรับผู้ใช้งานทั่วไป**

```bash
cd KUSE-ACTIVITY
npm run dev
```

**ระบบสำหรับผู้ดูแล**

```bash
cd KUSE-ADMIN-ACTIVITY
npm run dev
```

**ระบบ API**

```bash
cd API-MANAGE-ACTIVITY
npm run dev
```
