# Frequency Piano • keyboard2543

เว็บแอปเปียโนและเครื่องมือความถี่เสียงแบบ interactive

**URL ที่จะได้:** https://keyboard2543.github.io/frequency-piano

## คุณสมบัติหลัก

- **โหมดกดเปียโน** (Piano Mode)
  - คีย์บอร์ดเปียโน 2 อ็อกเทฟเต็ม (C4 ถึง C6)
  - แต่ละปุ่มแสดงชื่อโน้ต + ความถี่ (Hz) อย่างชัดเจน
  - กด/แตะแล้วเล่นเสียงทันที (Web Audio API)
  - รองรับการเลื่อนซ้ายขวาบนมือถือ

- **โหมดกำหนดความถี่** (Frequency Mode)
  - ป้อนหรือเลื่อนปรับความถี่ได้แบบเรียลไทม์
  - กดเล่นแล้วปรับความถี่ขณะเสียงดังอยู่ได้เลย
  - มีปุ่ม Preset โน้ตมาตรฐาน (C4, E4, G4, A4, C5 ฯลฯ)
  - เสียงจะค่อยๆ หยุดอย่างนุ่มนวลเมื่อกด Stop

## การใช้งานบนมือถือ (Full Screen)

- ออกแบบให้เต็มจอและใช้งานง่ายด้วยนิ้ว
- ปุ่มมีขนาดใหญ่พอสำหรับการแตะ
- คีย์บอร์ดสามารถเลื่อนซ้ายขวาได้สะดวก
- ใช้ Tailwind + responsive design

## วิธีนำขึ้น GitHub Pages

1. สร้าง Repository ใหม่ชื่อ `frequency-piano` (Public)
2. อัปโหลดไฟล์ `index.html` ไปที่ root ของ repo
3. ไปที่ **Settings → Pages**
4. เลือก **Source** เป็น `Deploy from a branch`
5. เลือก Branch: `main` และ Folder: `/ (root)`
6. กด **Save** รอสักครู่ เว็บจะขึ้นที่ `https://keyboard2543.github.io/piano-frequency`

## เทคโนโลยีที่ใช้

- HTML + Tailwind CSS (CDN)
- Vanilla JavaScript
- Web Audio API (Oscillator + Gain + Filter)
- Font Awesome icons

สร้างโดย keyboard2543 | 1 กรกฎาคม 2026

---

**Tips การใช้งาน:**
- บนคอมพิวเตอร์: กดปุ่มเปียโนด้วยเมาส์ หรือจะกดปุ่มบนคีย์บอร์ดคอมพิวเตอร์ก็ได้ (ในอนาคต)
- ความถี่อ้างอิงมาตรฐาน: **A4 = 440 Hz**
- เสียงเป็นแบบ Sine wave บริสุทธิ์ เหมาะสำหรับการเรียนรู้ความถี่