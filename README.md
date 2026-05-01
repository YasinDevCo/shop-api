# 🛍️ Shop API

یک API قدرتمند و مقیاس‌پذیر برای مدیریت فروشگاه آنلاین با قابلیت‌های کامل احراز هویت، محصولات، سبد خرید، پرداخت و مدیریت محتوا.

## ✨ قابلیت‌ها

- 🔐 **احراز هویت و مجوزدهی** (JWT Token)
- 👤 **مدیریت کاربران** (پروفایل، نقش‌ها، آدرس‌ها)
- 📦 **مدیریت محصولات** (CRUD، دسته‌بندی، جستجو، فیلتر)
- 🛒 **سبد خرید و سفارشات**
- 💳 **درگاه پرداخت**
- ⭐ **سیستم امتیازدهی و نظرات**
- ❤️ **لیست علاقه‌مندی‌ها (Wishlist)**
- 📝 **سیستم وبلاگ**
- 📊 **داشبورد مدیریتی**
- 📞 **فرم تماس**

## 🛠️ تکنولوژی‌ها

- **Runtime**: Node.js
- **Framework**: Express.js 5.x
- **Language**: TypeScript
- **Database**: MongoDB
- **ODM**: Mongoose 9.x
- **Authentication**: JWT + bcryptjs
- **Security**: CORS, Cookie Parser

## 📋 پیش‌نیازها

- **Node.js** >= 18.x
- **npm** >= 9.x یا **yarn** >= 1.22.x
- **MongoDB** >= 6.x
- **Git**

## 🚀 نصب و راه‌اندازی

### 1. کلون کردن پروژه


git clone https://github.com/your-username/shopapi.git
cd shopapi


### 2.نصب وابستگی‌ها
npm install
### 3.تنظیم متغیرهای محیطی
PORT=5000
MONGO_URI=mongodb://localhost:27017/shopapi
NODE_ENV=development
JWT_SECRET=your_super_secret_key_change_this
JWT_EXPIRES_IN=7d
FRONTEND_URL=http://localhost:3000
### 4.اجرا در حالت توسعه
npm run dev
### 5.ساخت نسخه تولید
npm run build
npm start

```bash


