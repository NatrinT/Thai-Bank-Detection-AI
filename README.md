🇹🇭 Thai Banknote Detection with YOLOv8

This project detects Thai Baht banknotes (20, 50, 100, 500, 1000 Baht) using the YOLOv8 object detection model. Dataset annotations are created with LabelImg in YOLO format.

📌 Features

Detects 5 types of Thai banknotes

Uses Ultralytics YOLOv8 for detection and training

Dataset labeling via LabelImg (YOLO format)

🏷️ Dataset Labeling with LabelImg

This project uses LabelImg to draw bounding boxes and create YOLO-format annotations for each banknote image.

🔧 How to Use LabelImg

Install LabelImg

pip install labelImg


หรือดาวน์โหลด GUI จาก GitHub:

https://github.com/heartexlabs/labelImg

เปิดโปรแกรม

labelImg


ตั้งค่า YOLO Format

ไปที่ View → Auto Save Mode

ไปที่ Yolo เพื่อเลือกให้เซฟเป็น YOLO TXT format

เริ่ม Label รูป

คลิก Create RectBox เพื่อวาดกรอบรอบธนบัตร

เลือกคลาส เช่น

20

50

100

500

1000

บันทึกไฟล์

ระบบจะสร้างไฟล์ .txt คู่กับไฟล์รูปแบบ YOLOv8:

class x_center y_center width height


โครงสร้าง Dataset

dataset/
  images/
    train/
    val/
  labels/
    train/
    val/

🚀 Train and Test on Google Colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Aeq77SH6MFBccXbQGgADBObeWNJhKglU?usp=sharing)
