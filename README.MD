# My Business Web - IT Solutions Partner

## คำอธิบายโครงการ

* เว็บไซต์ธุรกิจของ **IT Solutions Partner** (บริษัทรับทำเว็บไซต์และโซลูชันไอที)
* สร้างขึ้นเพื่อส่งงาน Assignment #1 โดยเน้นการสร้างเว็บไซต์แบบ Static พื้นฐาน
* เน้นการใช้ **HTML Semantic** ที่ถูกต้อง (ตามข้อกำหนดโดยยังไม่เน้น CSS หรือ JavaScript ซับซ้อน)
* เรียนรู้การจัดโครงสร้างหน้าเว็บ (Layout), การลิงก์ระหว่างหน้า (Navigation), และการสร้างฟอร์ม

## การอัปเดตล่าสุด (สรุป)

- รวม CSS หลักไว้ใน `css/styles.css` และปรับโครงสร้าง/จัดหมวดให้ชัดเจน (RESET, TYPOGRAPHY, LAYOUT, COMPONENTS, MEDIA QUERIES)
- ปรับปรุงการจัดวางด้วย Flexbox และ CSS Grid:
	- Navigation: ใช้ `display: flex` และ `justify-content: space-between` เพื่อจัด logo/เมนู
	- Services: `.services` เป็น Flex container; `.service-card` เป็น responsive item
	- Team: `.team` เป็น CSS Grid (`repeat(auto-fit, minmax(250px,1fr))`)
	- Contact form: ฟอร์มตั้งเป็น column flex กับ `gap: 15px` และ input กว้าง `100%`
- Interaction / UX:
	- ปุ่ม (`.btn`) มี hover lift, color change และ shadow
	- การ์ด (`.card`, `.service-card`, `.team-member`) มี smooth hover lift + shadow
	- เมนูมี hover effects และโครงสร้างซับเมนูพื้นฐาน
- Layout / positioning:
	- Header เป็น `position: sticky` ด้านบน
	- Hero ปรับให้ข้อความไม่ทับปุ่มโดยใช้ flex spacing (และ overlay เพิ่มความคมของข้อความ)
	- เพิ่มปุ่ม `#back-to-top` และ `#chat-widget` พร้อม CSS/JS พื้นฐาน

## ไฟล์ที่ถูกปรับปรุง (สำคัญ)
- `css/styles.css` — โครงสร้างใหม่, ตัวแปรสี, components, responsive rules, interaction effects
- `index.html`, `about.html`, `services.html`, `contact.html` — ลิงก์ไปยัง `css/styles.css`, header/footer/hero/sections ถูกจัดให้สอดคล้องกับ stylesheet, เพิ่ม markup สำหรับ widgets

หมายเหตุ: รูปภาพที่อ้างอิงต้องอยู่ในโฟลเดอร์ `images/` เพื่อให้ hero/team แสดงผลถูกต้อง

## ไฟล์ที่สร้าง

* **index.html** - หน้าแรกของเว็บไซต์ แสดงส่วน Hero Banner, บริการแนะนำ (Featured Services)
* **about.html** - หน้าข้อมูลบริษัท: ประวัติความเป็นมา, ทีมงานผู้เชี่ยวชาญ, และวิสัยทัศน์องค์กร
* **services.html** - หน้าแสดงรายละเอียดบริการ (Web Dev, SEO, Support) และตารางเปรียบเทียบราคาแพ็กเกจ
* **contact.html** - หน้าติดต่อเรา มีฟอร์มส่งข้อความ, ที่อยู่สำนักงาน, และ Google Maps

## โครงสร้างหน้าเว็บ (ตามความต้องการของลูกค้า)

### 1. หน้าแรก (index.html)
* 1.1 Header (Logo / ชื่อบริษัท IT Solutions Partner)
* 1.2 Navigation menu (หน้าแรก, เกี่ยวกับ, บริการ, ติดต่อ)
* 1.3 Hero section (ขนาดใหญ่ เนื้อหา Welcome สู่โลกเทคโนโลยี)
* 1.4 Featured services (3 บริการหลัก: Web Design, Digital Marketing, IT Support)
* 1.5 Footer

### 2. หน้า About (about.html)
* 2.1 เรื่องราวของบริษัท (Company Story)
* 2.2 ทีมงาน (ใช้ `<figure>` สำหรับรูปโปรไฟล์ Developer และ CEO)
* 2.3 Mission/Vision (พันธกิจและวิสัยทัศน์)
* 2.4 Link กลับหน้าแรก

### 3. หน้า Services (services.html)
* 3.1 รายการบริการทั้งหมด
* 3.2 ใช้ `<section>` แยกสำหรับแต่ละบริการ
* 3.3 Table เปรียบเทียบแพ็กเกจราคา (Starter vs Pro vs Enterprise)

### 4. หน้า Contact (contact.html)
* 4.1 มี Contact Form สำหรับกรอกข้อมูล (ชื่อ, อีเมล, ข้อความ)
* 4.2 ที่อยู่ของบริษัท (Address)
* 4.3 แผนที่ (Embedded Google Maps)

## All pages with direct links

| หน้า | ลิงก์ | รูปภาพตัวอย่าง |
| :--- | :--- | :--- |
| **[หน้าแรก](index.html)** | `index.html` | ![หน้าแรก](images/index.png) |
| **[เกี่ยวกับ](about.html)** | `about.html` | ![เกี่ยวกับ](images/about.png) |
| **[บริการ](services.html)** | `services.html` | ![บริการ](images/services.png) |
| **[ติดต่อ](contact.html)** | `contact.html` | ![ติดต่อ](images/contact.png) |


## How to Run

1.  เปิด `index.html` ใน Browser (Chrome, Edge, Firefox) เพื่อดูผลลัพธ์
2.  หรือเปิดผ่าน **Live Server** ใน VS Code เพื่อจำลอง Local Server

## ตรวจสอบ (Recommended quick checks)

1. เปิด `index.html` ที่ความกว้างหน้าจอเดสก์ท็อป — ตรวจดูว่า header ติดด้านบนและเมนูอยู่ขวา
2. ตรวจให้แน่ใจว่า Hero หัวเรื่องไม่ทับปุ่ม และข้อความอ่านได้ (contrast)
3. ไปที่ `services.html` — รายการบริการควรเรียงเป็น 3 คอลัมน์บน desktop และพับลงบนมือถือ
4. ไปที่ `about.html` — ทีมงานแสดงเป็น card grid แบบ responsive
5. ไปที่ `contact.html` — ฟอร์มมี spacing (`gap`) และ input เต็มความกว้าง

## ถ้าต้องการปรับเพิ่มเติม
- ต้องการเมนูแบบ hamburger สำหรับมือถือไหม (ผมจะเพิ่ม JS เล็กน้อย)
- ต้องการเอฟเฟกต์ fade/slide สำหรับ sub-menu หรือปรับคอนทราสต์/ตัวอักษรเพิ่มเติมไหม

---
Updated: 2025-12-19