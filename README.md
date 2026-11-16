# 📱 Kotlin Lab Assignments

รวมงานแลปการเขียนแอป Android ด้วย **Kotlin** และ **Jetpack Compose**

แต่ละโฟลเดอร์เก็บเฉพาะไฟล์ซอร์สโค้ดหลักของแต่ละงาน ไม่ใช่โปรเจกต์ Android Studio ที่เปิดรันได้ทันที

## 📂 งานแต่ละชิ้น

| โฟลเดอร์ | หัวข้อ | สิ่งที่ฝึก |
|---|---|---|
| [`ass6scaffold`](ass6scaffold) | Scaffold และ Navigation | โครงหน้าจอด้วย `Scaffold`, สลับหน้าด้วย Navigation Compose (`NavGraph`, `Screen`) |
| [`ass7dialoglazycolumn`](ass7dialoglazycolumn) | Dialog และ LazyColumn | แสดงรายการสมาชิกด้วย `LazyColumn` ใช้ `AlertDialog` เพิ่มสมาชิกและยืนยันการลบ |
| [`ass8mysql`](ass8mysql) | เชื่อมต่อ MySQL | แอปจัดการพนักงานผ่าน REST API (Retrofit + ViewModel) ฝั่งเซิร์ฟเวอร์เป็น Node.js (`server.js`) กับ MySQL (`sql.txt`) |

## 🛠️ เทคโนโลยี

`Kotlin` `Jetpack Compose` `Navigation Compose` `ViewModel` `Retrofit` `Node.js` `MySQL`

## 🚀 วิธีลองรัน

1. สร้างโปรเจกต์ใหม่ใน Android Studio แบบ **Empty Activity (Compose)**
2. คัดลอกไฟล์ `.kt` ของงานที่ต้องการ แก้ `package` และ `import` ให้ตรงกับโปรเจกต์ แล้วเพิ่ม dependency ที่งานใช้ใน Gradle (Navigation Compose สำหรับ `ass6scaffold`, Retrofit + Gson converter และ ViewModel สำหรับ `ass8mysql`)
3. สำหรับ `ass8mysql` ให้สร้างตารางตาม `sql.txt` ติดตั้งแพ็กเกจด้วย `npm install express mysql dotenv` ตั้งค่าการเชื่อมต่อฐานข้อมูล แล้วรัน `node server.js` จากนั้นแก้ URL ใน `EmployeeClient.kt` ให้ชี้ไปที่เซิร์ฟเวอร์ และเพิ่มสิทธิ์ `INTERNET` ใน `AndroidManifest.xml`
