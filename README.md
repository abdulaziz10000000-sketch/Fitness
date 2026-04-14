# COACH PRO - منصة التدريب الشخصي

## خطوات النشر (15 دقيقة فقط)

### 1. إعداد Firebase
1. افتح: https://console.firebase.google.com
2. Add project → اكتب "coachpro"
3. Realtime Database → Create database → اختر أقرب منطقة
4. Rules → اضع: { "rules": { ".read": true, ".write": true } }
5. Project Settings → Your apps → </> → انسخ firebaseConfig
6. افتح src/firebase.js وضع البيانات بدل YOUR_...

### 2. رفع على GitHub
1. github.com → New repository → اسمه "coachpro"
2. افتح Terminal في مجلد المشروع:
   git init
   git add .
   git commit -m "COACH PRO v1"
   git branch -M main
   git remote add origin https://github.com/USERNAME/coachpro.git
   git push -u origin main

### 3. النشر على Vercel
1. vercel.com → سجّل بـ GitHub
2. Add New Project → اختر coachpro
3. Framework: Create React App
4. Deploy ← ينتهي خلال دقيقتين

رابطك: https://coachpro.vercel.app

---

## بيانات الدخول
| النوع    | username     | password    |
|---------|--------------|-------------|
| مدرب    | coach_admin  | Admin@2025  |
| متدرب 1 | ahmed        | pass123     |
| متدرب 2 | khaled       | pass123     |
| متدرب 3 | fahad        | pass123     |

## لتغيير كلمة مرور المدرب
افتح src/App.jsx → ابحث عن TRAINER_CREDS → غيّر pass

## لإضافة متدرب جديد
سجّل دخول كمدرب → تبويب المتدربين → إضافة متدرب
