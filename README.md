# NGINX-install

NGINX เป็น Web Server ยอดนิยม โดยผู้ใช้งานแต่เดิมจะมีอยู่สองกลุ่ม กลุ่มแรกใช้ NGINX เป็น Web Server กลุ่มที่สองใช้งานเหมือนอุปกรณ์ไว้สำหรับ ‘ทดสอบ’ สิ่งต่าง ๆ ตามต้องการ

1.Install NGINX in Ubuntu

sudo apt install nginx


![image](https://github.com/thanawut2903/NGINX-install/assets/159118913/94143b9b-717d-424e-b2a6-f63c65c63275)


2.Start Service ของ NGINX และเมื่อ reboot ให้ start NGINX ด้วย

systemctl enable --now nginx

ตรวจสอบสถานะว่า NGINX พร้อมใช้งาน

systemctl status nginx

![image](https://github.com/thanawut2903/NGINX-install/assets/159118913/b6cb9576-7d13-4e65-babf-e3f435d9be2f)

3.อนุญาตให้คนนอกเข้ามาได้ ตัวอย่างที่ Port 80 TCP

firewall-cmd --permanent  --add-service http

firewall-cmd --reload

![image](https://github.com/thanawut2903/NGINX-install/assets/159118913/d0e21819-f12b-46a4-8518-93ded280f1a3)



