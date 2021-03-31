# การทดลองที่ 7 เรื่อง การเขียนโปรแกรมสร้างไวไฟ(WiFi AP)

## วัตถุระสงค์ 
เพื่อการเขียนโปรแกรมสร้าง WiFi AP

## อุปกรณ์ที่ใช้
1. Notebook
2. ไมโครคอนโทรเลอร์
3. USB
4. serial

## ศึกษาข้อมูลเบื้องต้น
* [วิธีการทดลอง] (https://www.youtube.com/watch?v=T26DVHePlTs&ab_channel=TANI-IOT)
* [Source code] (https://github.com/choompol-boonmee/lab63b/tree/master/examples)
* [platformio] (https://platformio.org/)

## วิธีการทดลอง
1. ต่อUSBและไมโครคอนโทรเลอร์เข้ากับ serial
![S__4948024](https://user-images.githubusercontent.com/80882549/113194512-6c4c9600-928b-11eb-8ded-7fe70398bd3e.jpg)

2. เตรียมโปรแกรมที่จะอัปโหลดเข้าไปในไมโครคอนโทรเลอร์ โดยเริ่มจากตั้งชื่อWiFi และ password หลังจากนั้นกำหนด IP address ของตัวเอง , gateway เป็นอะไร และ subnet เป็นยังไง
![S__4948026](https://user-images.githubusercontent.com/80882549/113194566-7a021b80-928b-11eb-8130-4a4c4ae66117.jpg)

3. เตรียม WEbserver ไว้ 1 ตัว รันคำสั่ง WiFi.softAP แล้วกำหนด ssid กับ password ลงไป
![S__4948027](https://user-images.githubusercontent.com/80882549/113194608-84bcb080-928b-11eb-8f58-c6a8fe1ddb95.jpg)

4.  บอกว่า IP ที่ตั้งไว้เป็นเท่าไร
![S__4948028](https://user-images.githubusercontent.com/80882549/113194656-8dad8200-928b-11eb-83de-426c009d00e1.jpg)

5.  อัปโหลดโปรแกรมเข้าไปในไมโครคอนโทรเลอร์
![S__4948029](https://user-images.githubusercontent.com/80882549/113194688-97cf8080-928b-11eb-8efb-6a7e26a2ea68.jpg)

6.  กดปุ่ม upload และ reset
![S__4948030](https://user-images.githubusercontent.com/80882549/113194735-a158e880-928b-11eb-9373-a184e377739a.jpg)

7.  รันคำสั่ง pio device monitor
![S__4948031](https://user-images.githubusercontent.com/80882549/113194760-a9188d00-928b-11eb-9792-249dc3b443bd.jpg)

## การบันทึกผลการทดลอง
จากการทำการทดลองข้างต้นเมื่ออัปโหลดโปรแกรมเสร็จสามารถตรวจสอบโดยใช้โทรศัพท์มือถือในการค้รหา WiFi ถ้าจะเชื่อมต่อก็กดเข้าไปแล้วใส่รหัสที่ตั้งไว้เพื่อเชื่อมต่อ

## อภิปรายผลการทดลอง
จากการทดลองการเขียนโปรแกรมนี้เป็นการฝึกสร้าง WiFi ซึ่งการทดลองจะคล้ายๆกับแลปที่5แต่ต่างจากตัวอย่างที่5ตรงที่สร้าง WiFi AP ขึ้นมาเอง

## คำถามหลังการทดลอง
1. เปิด Webserver ที่ port เท่าไร
  * ที่ port80
2. ตัวโปรแกรมมีการวน loop หรือไม่
  * ไม่มีการใช้คำสั่ง loop
