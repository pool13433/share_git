# workshop 3

## exercise 3.1  case study ต่าง ๆ ที่พบเจอ
### 3.1.1 .gitignore เพื่อทำให้ git ไม่สนใจไฟล์ที่เปลี่ยนแปลง ตัวอย่างไฟล์ .gitignore
```
public/*
*.js
*.css
```
[https://git-scm.com/docs/gitignore]
### 3.1.2 กรณีต้องการเพิ่มไฟล์ใส่ gitignore แต่ไฟล์เคย push ไป ที่ remote repo ไปแล้ว ต้อง reset (clear local cache repo ก่อน )
```
git rm --rf --cached .
git add .
```
### 3.1.3 save credential global ไม่ต้องใส่ password จะครั้งที่ push
```
$ git config credential.helper store
$ git push http://example.com/repo.git
Username: <type your username>
Password: <type your password>

[several days later]
$ git push http://example.com/repo.git
[your credentials are used automatically]
```

### 3.1.4 สร้างไฟล์ README.md ใส่คำอธิบาย repo เหมือนไฟล์นี้
(เรียนเขียน markdown lang)[https://dillinger.io/]