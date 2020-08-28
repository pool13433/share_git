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
### 1.2.2  สร้างไฟล์ {ชื่อเลนตัวเองeng}.txt และ ตรวจสอบสถานะ git อีกครั้ง เพื่อดูความเปลี่ยนแปลง
```
git status 
```
### 1.2.3  เพิ่มไฟล์เข้าไปที่ staged
```
git add {ชื่อเลนตัวเองeng}.txt  // ระบุชื่อเฉพาะ
git add .     // เพื่อ add ทุกอย่าง
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
## สุดท้ายจะได้ไฟล์