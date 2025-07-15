# ตัวแปลงค่าเงิน (Currency Converter)

เว็บแอปพลิเคชันสำหรับแปลงค่าเงินบาทไทยเป็นบิตคอยน์ พร้อมอัตราแลกเปลี่ยนสด

## คุณสมบัติ

- แปลงค่าเงินบาท (THB) ↔ บิตคอยน์ (BTC)
- อัตราแลกเปลี่ยนสดสำหรับ Bitcoin, ทองคำ, และดอลลาร์
- ระบบสมัครสมาชิกและเข้าสู่ระบบ
- ดีไซน์ที่ตอบสนอง (Responsive Design)
- โหมดมืด (Dark Mode)

## การติดตั้ง

### ตัวเลือกที่ 1: ใช้ไฟล์ที่ compile แล้ว (แนะนำ)
1. Clone repository นี้
2. เปิดไฟล์ `index.html` ในเบราว์เซอร์
3. ไฟล์ CSS ถูก compile ไว้แล้วใน `dist/output.css`

### ตัวเลือกที่ 2: Development mode
1. ติดตั้ง Node.js และ npm จาก [https://nodejs.org/](https://nodejs.org/)
2. Clone repository นี้
3. ติดตั้ง dependencies:

```bash
npm install
```

## การใช้งาน

### วิธีที่ 1: เปิดไฟล์โดยตรง (แนะนำ)
```bash
# เปิดไฟล์ index.html ในเบราว์เซอร์
# หรือใช้ Live Server extension ใน VS Code
```

### วิธีที่ 2: Development Mode (ต้องติดตั้ง Node.js)
```bash
npm run dev
```

### วิธีที่ 3: Production Build (ต้องติดตั้ง Node.js)
```bash
npm run build:prod
```

### วิธีที่ 4: Start Local Server (ต้องติดตั้ง Node.js)
```bash
npm start
```

## การแก้ปัญหา

### ปัญหา: "Specified input file ./src/input.css does not exist"
**สาเหตุ**: Node.js ไม่ได้ติดตั้ง หรือ path ไม่ถูกต้อง

**วิธีแก้**:
1. ติดตั้ง Node.js จาก [https://nodejs.org/](https://nodejs.org/)
2. รันคำสั่ง `npm install` ก่อน
3. หรือใช้ไฟล์ที่ compile ไว้แล้วใน `dist/output.css`

### ปัญหา: Build failed
**วิธีแก้**:
1. ตรวจสอบว่า Node.js ติดตั้งแล้ว
2. ลบโฟลเดอร์ `node_modules` และรัน `npm install` ใหม่
3. หรือใช้ไฟล์ `build.bat` ที่สร้างไว้

## โครงสร้างโปรเจค

```
├── index.html          # ไฟล์หลัก
├── src/
│   └── input.css      # Tailwind CSS input
├── dist/              # Compiled CSS (generated)
├── package.json       # Dependencies และ scripts
├── tailwind.config.js # Tailwind configuration
└── postcss.config.js  # PostCSS configuration
```

## เทคโนโลยีที่ใช้

- HTML5
- CSS3 (Tailwind CSS)
- JavaScript (ES6+)
- PostCSS
- Google Fonts (Sarabun)

## API ที่ใช้

- CoinGecko API สำหรับข้อมูล cryptocurrency
- GoldPrice API สำหรับข้อมูลทองคำ

## การพัฒนา

1. แก้ไขไฟล์ `index.html` สำหรับ HTML
2. แก้ไขไฟล์ `src/input.css` สำหรับ CSS custom
3. รัน `npm run dev` เพื่อ compile CSS แบบ watch mode
4. เปิดไฟล์ `index.html` ในเบราว์เซอร์

## License

MIT License 