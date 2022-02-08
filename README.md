# CLIP1
## 1 digital
การใช้ข้อมูล digital คือการเอาสัญญาณไฟฟ้ามาแทนตัวเลข ซึ่งเป็นตัวเลขฐาน2 มีเพียง 0 และ 1 

0 คือ 0ff หรือ 0 V และ 1 คือ on หรือ V สูงสุด
## 2 voltage
แรงดันไฟฟ้า คือความต่างศักย์ไฟฟ้าระหว่างจุด 2 จุด หน่อยเป็น V 

มีทั้งหมด 2 ประเภท คือ 1. แรงดันไฟฟ้ากระแสสลับ (เช่น ไฟบ้าน ประมาณ 230 V)  2. แรงดันไฟฟ้ากระแสตรง (เช่น แบตเตอร์รี่ เครื่องคอมพิวเตอร์(USB))
## 3 computer
เมื่อประมาณ 60 ปีที่แล้ว คอมพิวเตอร์เคยมีขนาดเทียบเท่ากับตึก 1 ตึก แต่ปัจจุบันก็มี ทั้งขนาดใหญ่ ขนาดกลาง และขนาดเล็ก 
## 4 internet
internet ทำให้ทุกๆอย่างสามารถเชื่อมโยงกันได้ มีทั้งไร้สาย และ มีสาย
## 5 program lang
การเขียนโปรแกรมมีวิวัฒนาการมาตั้งแต่ 50-70 ปีที่แล้ว ตั้งแต่ภาษา C และได้วิวัฒนาการมาเรื่อยๆเป็นจำนวนมากเพื่อให้คนสามารถเขียนภาษาและพัฒนาโปรแกรมได้ง่ายมากขึ้น
## 6 platformio
platformio เป็นการพัฒนามาตรฐานแบบใหม่แบบเปิด ที่ใช้วิธีการเขียนโปรแกรมแบบเดียวแต่สามารถเขียนลงบน microcontroller ได้หลายแบบ
## การทดลองที่ 1 เรื่อง การเขียนโปรแกรมเพื่อรันบนไมโครคอนโทรเลอร์
จะใช้โปรแกรมตัวอย่าง 01 serial จะมี 2 function คือ

1. setup จะ run ครั้งเดียว ซึ่งจะ set serial ที่ความเร็ว 115200

2.loop จะ run วนตลอดไป ซึ่งจะทำให้เพิ่มตัวแปร count ขึ้นเรื่อยๆ โดยให้แสดงผลเป็นตัวแปร count ออกมา ที่ช่วงเวลา 1 s 

จากนั้นก็ runและ upload โปรแกรม แล้วขณะที่ run ก็กด reset ไมโครคอนโทรเลอร์ และ device mornitor และดูผลลัพธ์ที่แสดงออกมาบนคอมพิวเตอร์
## การทดลองที่ 2 เรื่อง การเขียนโปรแกรมค้นหาไวไฟ
ตัวโปรแกรมก็จะมี 2 function เหมือนการทดลองที่ 1 ซึ่งในส่วน setup จะ set ในส่วนของ wifi ให้พร้อมทำงาน 

แต่ในส่วน loop ก็ให้วนตลอดไปให้แสดงผลค้นหา wifi พอได้ wifi ก็ให้แสดงผลว่ามี wifi รอบตัวอะไรบ้าง

runและ upload โปรแกรม แล้วขณะที่ run ก็กด reset ไมโครคอนโทรเลอร์ และ device mornitor และดูผลลัพธ์ที่แสดงออกมาบนคอมพิวเตอร์ ว่าเจอ wifi อะไรบ้าง
## การทดลองที่ 3 เรื่อง การเขียนโปรแกรมเอ้าพุทสัญญาณดิจิทัล
จะมีการใช้ adapter เสียบก่อน แล้วค่อยใช้ไมโครคอนโทรเลอร์ต่อบน adapter อีกที

การเขียนจะมี 2 function เหมือนการทดลองที่ 1 ซึ่งในส่วน setup จะ set ให้ 0 เป็น output 

แต่ในส่วน loop ก็ให้วนตลอดไป โดยวนทุกครึ่งวินาที ซึ่งเพิ่มตัวแปร count ขึ้นเรื่อยๆ 

ถ้า count เป็นคี่ ก็จะ on แล้วก็จะส่งค่าที่สูงที่สุดไป (1) และถ้า count เป็นคู่ก็จะเป็น off แล้วก็จะส่งค่าต่ำสุดไป (0)
และทำการ run เหมือนการทดลองที่ 1 ก็จะแสดง on-off ออกมา

จากนั้นเมื่อใช้ไมโครคอนโทรเลอร์มาต่อกับตัว delay เพื่อใช้ในการเปิด-ปิดสวิตช์อุปกรณ์ไฟฟ้าที่ใช้ในบ้านได้ 

จะได้ยินเสียงหน้าสัมผัสของสัญญาณไฟเปิด-ปิดนั้นด้วยเมื่อนำ delay ไปต่อกับแหล่งจ่ายไฟ
## การทดลองที่ 4 เรื่อง การเขียนโปรแกรมอินพุทสัญญาณดิจิทัล
โปรแกรมก็จะมี 2 function เหมือนการทดลองที่ 1 ซึ่งในส่วน setup จะ set ให้ 0 เป็น input และ 2 เป็น output

แต่ในส่วน loop ก็ให้วนตลอดไป จะอ่านสัญญาณ digital (0) 

ถ้าเป็น 1 จะทำให้ 2 (output) ไฟดับ และถ้าเป็น 0 (output) ไฟติด

และทำการ run เหมือนการทดลองที่ 1 ก็จะแสดงสัญญาณ digital (0 หรือ 1)

จากนั้นเมื่อนำไปต่อกับเซนเซอร์แสงที่ต่ออยู่กับตัวต้านทาน 

เมื่อเซนเซอร์โดนแสงก็จะทำให้สัญญาณ digital เป็น 0 และทำให้ไฟติด แต่เมื่อเอานิ้วไปบังเซนเซอร์ให้ไม่โดนแสงก็จะทำให้สัญญาณ digital เป็น 1 และทำให้ไฟดับ
## ทดลองที่ 5 เรื่อง การเขียนโปรแกรมเชื่อมต่อไวไฟและเว็บเซอร์เวอร์
โปรแกรมจะต้องต่อกับ wifi จึงต้องใส่ชื่อและรหัสของ wifi ที่ใช้ไป 

หลังจากนั้นโปรแกรมก็จะมี 2 function เหมือนการทดลองที่ 1 

ซึ่งในส่วน setup จะเป็นการ connect กับ wifi ที่เลือกไว้ และ setup ตัว server ถ้ามีการเชื่อมโยงก็จะแสดง Hello count ซึ่งตัว count จะเพิ่มขึ้นเรื่อยๆ

และทำการ run เหมือนการทดลองที่ 1 
## การทดลองที่ 6 เรื่อง การเขียนโปรแกรมสร้างไวไฟแอคเซสพอยต์ (Wifi AP)
การทดลองนี้จะต่างจากการทดลองที่ 5 ตรงที่ว่า การทดลองครั้งที่ 5 จะเชื่อมโยงกับ wifi ที่มีอยู่แล้วเท่านั้น แต่การทดลองที่ 6 เป็นการสร้าง wifi ขึ้นมาเอง

โดยในโปรแกรมจะต้องตั้งชื่อและรหัสขึ้นมาเอง และต้องกำหนด IPAddress เป็นอะไร 

โปรแกรมก็จะมี 2 function เหมือนการทดลองที่ 1 

ในส่วน setup จะเป็นการเตรียม server ไว้ 1 ตัว และใช้คำสั่ง softAP จากนั้น กำหนด ssid , password และ IP ลงไป

และทำการ run เหมือนการทดลองที่ 1 และทดสอบโดยใช้โทรศัพท์มือถือว่ามี wifi ที่เราทำไว้หรือไม่
