# การรู้จำภาพตัวอักษร
# ชื่อกลุ่ม คนพันธุ์เสือใจเกเร
## รายชื่อสมาชิกกลุ่ม
1. นาย ปุลวัชร ลี้เจริญ 62070256
2. นาย วีรวัฒน์ บัวชุม 62070271
3. นาย สมิทธิ์ เฉียบแหลม 62070276
4. นาย สิริปกรณ์ วรวสุนธรา 62070280
## Project 2: Handcraft _base :)
### วิธี Run Code
```
handcraft_based.ipynb
```
  ต้องเปิดด้วย Google Colab โดยสร้างเป็น Folder ใน Google Drive เพื่อเก็บตัวไฟล์ handcraft_based.ipynb และ Folder Tr ที่เป็น Training image ไว้ด้วยกันและทำการ Mount Google Colab กับ Google Drive ที่ทำการเก็บไฟล์ Project 2
  
โดยในไฟล์ handcraft_based.ipynb จะมี 2 ส่วนหลักๆ 
   * Training - ใช้ HOG และ Radon ในการทำ Feature Extraction เมื่อ Run เสร็จ Progress Bar จะเป็น 100%
   * Testing - ใช้ K-Nearest Neighbors รู้จำภาพอักษร เมื่อ Run เสร็จจะแสดงการคำตอบในรูปแบบ Answer is [เลขของคลาสตัวอักษร]
### วิธีการเปลี่ยนรูป Dataset
   * ส่วนของ Training
      
      ![image](https://user-images.githubusercontent.com/56358092/119257555-f19b5980-bbef-11eb-889d-63e0b372f6f0.png)
      
      ให้ทำการวาง path ของ Folder รูปภาพ(Tr) ที่อยู่ใน Google Drive มาใส่แทน path ของเดิม => /content/drive/MyDrive/ImgRecPJ2/Tr/
   * ส่วนของ Testing
  
      ![image](https://user-images.githubusercontent.com/56358092/119257064-dc253000-bbed-11eb-9686-45e696cc9545.png) 
      
      ให้ทำการวาง path ใหม่ของรูปภาพที่ต้องการจะทดสอบ มาใส่แทน path ของเดิม => '/content/drive/MyDrive/ImgRecPJ2/ซ.png'



## Project 3: Learning_base :)
### วิธี Run Code
```
learning_based.ipynb
```
  ต้องเปิดด้วย Google Colab โดยสร้างเป็น Folder ใน Google Drive เพื่อเก็บตัวไฟล์ learning_based.ipynb และ Folder Tr ที่เป็น Training image ไว้ด้วยกันและทำการ Mount Google Colab กับ Google Drive ที่ทำการเก็บไฟล์ Project 3
  
โดยในไฟล์ learning_based.ipynb จะมี 2 ส่วนหลักๆ 
   * Import Library : ทำการ import library ที่สำคัญต่อการทำงาน
   * Data Loader : ทำการ Load dataset เข้ามาในระบบและปรับขนาดให้เป็น 128x128 (Gray scale)
   * Training & Validating Set Generation: ทำการแปลง format รูปภาพให้สามารถทำงานร่วมกับ pytorch และแบ่งข้อมูลสำหรับการสอน Model 90%
   * CNN Model : ในส่วนนี้จะเป็นส่วนของโครงสร้างการสกัดหา feature 
   * Defining Learning Algorithm : วิธีการที่ใช้ในการจัดการกับค่าที่ Model คำนวนผิดพลาดเพื่อไปทำการใช้ต่อในส่วน backpropagation
   * Training Model : ทำการ train model ให้เรียนรู้กับข้อมูล train data ที่แบ่งไว้ 90% โดยในส่วนนี้จัดทำการสอน model 25 ครั้ง
   * Testing : ส่วนที่ใช้ทำการทดสอบความแม่นยำของข้อมูลที่ถูกแบ่งไว้ test 10%
   * Executing Model with Testing Image : ในส่วนนี้จะใช้ในการพยากรณ์เคสใหม่ที่ถูกส่งเข้าาให้ model ทำการจำแนก
### วิธีการเปลี่ยนรูป Dataset
   * ส่วนของ Training
      
      ![image](https://user-images.githubusercontent.com/57053814/119268046-4f916680-bc1b-11eb-9969-61df771f2ea3.png)
      
      ให้ทำการวาง path ของ Folder รูปภาพ(Tr) ที่อยู่ใน Google Drive มาใส่แทน path ของเดิม => /content/drive/MyDrive/ImgRecPJ2/Tr/
   * ส่วนของ Testing
  
      ![image](https://user-images.githubusercontent.com/56358092/119257064-dc253000-bbed-11eb-9686-45e696cc9545.png) 
      
      ให้ทำการวาง path ใหม่ของรูปภาพที่ต้องการจะทดสอบ มาใส่แทน path ของเดิม => '/content/drive/MyDrive/ImgRecPJ2/ซ.png'

