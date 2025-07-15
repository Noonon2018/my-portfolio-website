# ตัวแปลงค่าเงิน (Currency Converter)

เว็บแอปพลิเคชันสำหรับแปลงค่าเงินบาทไทยเป็นบิตคอยน์ พร้อมอัตราแลกเปลี่ยนสด

## คุณสมบัติ

- แปลงค่าเงินบาท (THB) ↔ บิตคอยน์ (BTC)
- อัตราแลกเปลี่ยนสดสำหรับ Bitcoin, ทองคำ, และดอลลาร์
- ระบบสมัครสมาชิกและเข้าสู่ระบบ
- ดีไซน์ที่ตอบสนอง (Responsive Design)
- โหมดมืด (Dark Mode)

## การติดตั้ง

1. ติดตั้ง Node.js และ npm
2. Clone repository นี้
3. ติดตั้ง dependencies:

```bash
npm install
```

## การใช้งาน

### Development Mode
```bash
npm run dev
```

### Production Build
```bash
npm run build:prod
```

### Start Local Server
```bash
npm start
```

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