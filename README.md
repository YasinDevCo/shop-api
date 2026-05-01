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



# ========== احراز هویت (Auth) ==========
POST   /api/auth/register
POST   /api/auth/login
POST   /api/auth/logout
GET    /api/auth/me
POST   /api/auth/refresh-token

# ========== کاربران (User) ==========
GET    /api/user/profile
PUT    /api/user/profile
PUT    /api/user/change-password
DELETE /api/user/delete

# ========== آدرس‌ها (Addresses) ==========
GET    /api/addresses
POST   /api/addresses
PUT    /api/addresses/:id
DELETE /api/addresses/:id

# ========== محصولات (Product) ==========
GET    /api/product
GET    /api/product/:id
POST   /api/product
PUT    /api/product/:id
DELETE /api/product/:id
GET    /api/product/search?q=

# ========== دسته‌بندی (Category) ==========
GET    /api/category
POST   /api/category
PUT    /api/category/:id
DELETE /api/category/:id

# ========== سفارشات (Orders) ==========
GET    /api/orders
GET    /api/orders/:id
POST   /api/orders
PUT    /api/orders/:id/cancel

# ========== پرداخت (Payment) ==========
POST   /api/payment/create
GET    /api/payment/verify
GET    /api/payment/status/:id

# ========== علاقه‌مندی‌ها (Wishlist) ==========
GET    /api/wishlist
POST   /api/wishlist/:productId
DELETE /api/wishlist/:productId

# ========== نظرات (Reviews) ==========
GET    /api/reviews/product/:productId
POST   /api/reviews/:productId
PUT    /api/reviews/:id
DELETE /api/reviews/:id

# ========== وبلاگ (Blogs) ==========
GET    /api/blogs
GET    /api/blogs/:id
POST   /api/blogs
PUT    /api/blogs/:id
DELETE /api/blogs/:id

# ========== تماس (Contact) ==========
POST   /api/contact
GET    /api/contact

# ========== داشبورد (Dashboard) ==========
GET    /api/dashboard/stats
GET    /api/dashboard/users
GET    /api/dashboard/sales

```bash


