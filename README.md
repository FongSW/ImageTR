# ImageTR
# ชื่อกลุ่ม คนพันธุ์เสือใจเกเร
## รายชื่อสมาชิกกลุ่ม
1. นาย ปุลวัชร ลี้เจริญ 62070256
2. นาย วีรวัฒน์ บัวชุม 62070271
3. นาย สมิทธิ์ เฉียบแหลม 62070276
4. นาย สิริปกรณ์ วรวสุนธรา 62070280
## Project 2: Handcraft _base :)
### วิธี Run Code
```
  python handcraft_based.ipynb
```
  ต้องเปิดด้วย Google Colab โดยสร้างเป็น Folder ใน Google Drive เพื่อเก็บตัวไฟล์ handcraft_based.ipynb และ Folder Tr ที่เป็น Training image ไว้ด้วยกันและทำการ Mount Google Colab กับ Google Drive ที่ทำการเก็บไฟล์ Project 2
  
โดยในไฟล์ handcraft_based.ipynb จะมี 2 ส่วนหลักๆ 
   * Training - ใช้ HOG และ Radon ในการทำ Feature Extraction เมื่อ Run เสร็จ Progress Bar จะเป็น 100%
   * Testing - ใช้ K-Nearest Neighbors รู้จำภาพอักษร เมื่อ Run เสร็จจะแสดงการคำตอบในรูปแบบ Answer is [เลขของคลาสตัวอักษร]
### วิธีการเปลี่ยนรูป Dataset
   * ส่วนของ Training
      
      ![image](https://user-images.githubusercontent.com/56358092/119255026-b5fa9280-bbe3-11eb-9592-77b8e9c05730.png)
      
      ให้ทำการวาง path ของ Folder รูปภาพ(Tr) ที่อยู่ใน Google Drive มาใส่แทน path ของเดิม => /content/drive/MyDrive/ImgRecPJ2/Tr/
   * ส่วนของ Testing
  
      ![image](https://user-images.githubusercontent.com/56358092/119257064-dc253000-bbed-11eb-9686-45e696cc9545.png) 
      
      ให้ทำการวาง path ใหม่ของรูปภาพที่ต้องการจะทดสอบ มาใส่แทน path ของเดิม => '/content/drive/MyDrive/ImgRecPJ2/ซ.png'

