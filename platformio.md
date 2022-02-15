# วิธีการติดตั้ง platformio
## เว็บโหลด git
https://git-scm.com/download/win

## เว็บโหลด python
https://www.python.org/downloads/windows/

## เว็บโหลด nodejs
https://nodejs.org/en/download/

## วิธีติดตั้ง git คือ
1. เข้าเว็บโหลด git และคลิกที่ 64-bit Git for Windows Setup. แล้วติดตั้งบนเครื่องคอมพิวเตอร์
2. เปิด command prompt รันคำสั่ง git clone https://github.com/choompol-boonmee/iotset1.git
3. ติดตั้ง python และ nodejs ซึ่งตอนที่ติดตั้ง python ต้องคลิก ที่ add python to PATH ด้วย
4. รัน pip install -U platformio บน command prompt
5. รัน cd iotset1/examples และ dir ตามลำดับ บน command prompt เพื่อเข้าไปโฟลเดอร์ iotset1
6. ตรวจสอบ โฟลเดอร์ตัวอย่าง เช่น ถ้ารันตัวอย่างที่ 1 คือ cd iotset1/examples/ex01 และ pio run ตามลำดับ หรือ 

ถ้ารันตัวอย่างที่ 2 คือ cd iotset1/examples/ex03 และ pio run ตามลำดับ เป็นต้น
