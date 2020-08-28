# workshop 1

## exercise 1.1
``` 
git clone https://github.com/pool13433/share_git.git 
```

## exercise 1.2 
### 1.2.1 เพื่อแสดงสถานะล่าสุดของ git local repository
```
git status
git status -u
```
[http://schacon.github.io/git/git-status.html]
### 1.2.2  สร้างไฟล์ {user}.txt  (ตัวอย่าง poola410.txt) และ ตรวจสอบสถานะ git อีกครั้ง เพื่อดูความเปลี่ยนแปลง ตัวอย่าง poola410.txt
```
git status 
```
### 1.2.3  เพิ่มไฟล์เข้าไปที่ staged
```
git add {user}.txt  // ระบุชื่อเฉพาะ
git add .     // เพื่อ add ทุกอย่าง
```
### 1.2.4.1  ย้อนกลับ จาก ใช้คำสั่ง git add 
```
git reset
```
### 1.2.4.2  เผลอลบไฟล์ที่ local ให้ไปดึงไฟล์ที่ remote ลงมาใหม่
```
git checkout {fileที่ลบไป}
```
### 1.2.4  track โดยการเพิ่ม message กำกับ
```
git commit -m "first commit"
git status
```
### 1.2.5  push โยนไฟล์ local ไปที่ remote repository
```
git push origin master
```
### จะได้ไฟล์ {user}.txt อยู่บน github ที่ /workshop1/{user}.txt

## git คำสั่งเพิ่มเติมที่มีประโยชน์
### คำสั่งดูความแตกต่าง
```
git diff // เฉพาะ Branch หรือ Commit ID ที่เราใช้อยู่ ณ ขณะนี้
git diff <commit_id> // แบบระบุ Commit ID 
git diff <commit_id> <commit_id> // เปรียบเทียบระหว่างสอง Commit
```
### คำสั่งดู Log
```
git log
git log --oneline // แสดงแต่ละlog เหลือบรรทัดเดียว
git log --pretty=oneline // แสดงแต่ละlog เหลือบรรทัดเดียว แต่แสดง commit เต็มไม่ซ่อน 
git log --graph // แสดงเป็นเส้น Branch ให้ดูง่ายขึ้น
git log --oneline --graph // ถ้าใช้แบบนี้จะดูง่ายขึ้นมาก
```