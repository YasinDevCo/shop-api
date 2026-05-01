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
- **npm** >= 9.x
- **MongoDB** >= 6.x
- **Git**
## 🚀 نصب و راه‌اندازی

```bash
# 1. کلون کردن پروژه
git clone https://github.com/your-username/shopapi.git
cd shopapi

# 2. نصب وابستگی‌ها
npm install

# 3. ساخت فایل .env
echo "PORT=5000" > .env
echo "MONGO_URI=mongodb://localhost:27017/shopapi" >> .env
echo "NODE_ENV=development" >> .env
echo "JWT_SECRET=your_secret_key" >> .env
echo "JWT_EXPIRES_IN=7d" >> .env
echo "FRONTEND_URL=http://localhost:3000" >> .env

# 4. اجرا در حالت توسعه
npm run dev

# 5. ساخت نسخه تولید
npm run build
npm start
```

## 🌐 مسیرهای API (قابل کپی)

```bash
POST   /api/auth/register
POST   /api/auth/login
POST   /api/auth/logout
GET    /api/auth/me

GET    /api/user/profile
PUT    /api/user/profile
PUT    /api/user/change-password

GET    /api/addresses
POST   /api/addresses
PUT    /api/addresses/:id
DELETE /api/addresses/:id

GET    /api/product
GET    /api/product/:id
POST   /api/product
PUT    /api/product/:id
DELETE /api/product/:id

GET    /api/category
POST   /api/category
PUT    /api/category/:id
DELETE /api/category/:id

GET    /api/orders
GET    /api/orders/:id
POST   /api/orders

GET    /api/wishlist
POST   /api/wishlist/:productId
DELETE /api/wishlist/:productId

GET    /api/reviews/product/:productId
POST   /api/reviews/:productId

GET    /api/blogs
GET    /api/blogs/:id
POST   /api/blogs

POST   /api/contact

GET    /api/dashboard/stats
```

## 📝 تست سریع با cURL

```bash
# ثبت‌نام
curl -X POST http://localhost:5000/api/auth/register \
  -H "Content-Type: application/json" \
  -d '{"name":"test","email":"test@test.com","password":"123456"}'

# ورود
curl -X POST http://localhost:5000/api/auth/login \
  -H "Content-Type: application/json" \
  -d '{"email":"test@test.com","password":"123456"}'

# دریافت محصولات
curl -X GET http://localhost:5000/api/product
```

## 📄 لایسنس

ISC
