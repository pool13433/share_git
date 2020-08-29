# workshop 2

## exercise 2.1 git branching & merging
### 2.1.1 ตรวจสอบสถานะ branch ที่ local repo ปัจจุบัน
``` 
git branch
```
### 2.1.2  สร้าง local branch
```
git branch {branch_name}
```
### 2.1.3  เปลี่ยน branch 
```
git checkout -b {branch_name} // git ก่อน version 2.23
git switch {branch_name} // git version 2.23
```
### 2.1.4 merge branch switch ไปที่ branch ที่จะ merge (branch code เก่า) และ merge branch ใหม่ (branch code ใหม่)
```
git switch master
git merge dev_pool
```
### 2.1.4 การเก็บซ่อนการเปลี่ยนแปลงทั้งหมดไว้ทั้งหมด และสามารถนำกลับมาโดยใช้ git stash pop
```
git stash  // ซ่อน
git stash pop // ไม่ซ่อน
git stash list  // แสดงรายการ stash ทั้งหมด
```

### 2.1.4 tag 
```
git tag -a {tag_text} -m "message"
```

## exercise 2.2 แชร์โค๊ด และ การดึงโค๊ด
### 2.2.1  การตรวจสอบไฟล์ภายใน local และ remote แจ้งให้ทราบว่ามีการเปลี่ยนแปลงที่ local กับ remote ตรงกันหรือไม่
```
git fetch
```
### 2.2.2 ดึงโค๊ดจาก remote
```
git pull  // pull ตาม branch ที่เลือกอยู่
git pull origin master
```
### 2.2.3 ส่งโค๊ดของเราจาก local ไปที่ remote repo
```
git push origin master  // master คือ branch ที่ remote repo
```
