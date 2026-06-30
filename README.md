<p align="center">
<img src="https://img.shields.io/badge/Project-Vehicle%20Access%20Control%20System-blue?style=for-the-badge">
<img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
<img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
<img src="https://img.shields.io/badge/PlantUML-00599C?style=for-the-badge">
<img src="https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white">
</p>


# 🚗 Vehicle Access Control System (VACS)
## سیستم کنترل ورود و خروج خودرو

---

## 👤 اطلاعات پروژه

| | |
|--|--|
| **نام دانشجو** | خدیجه رکنی |
| **شماره دانشجویی** | 40213343 |
| **استاد** | دکتر سید مهرداد اسلامی مهدی آبادی |
| **درس** | تحلیل و طراحی نرم‌افزار |
| **سال تحصیلی** | 1405-1404 ( ترم بهمن ) |

---

## 📋 شرح سیستم

سیستم کنترل ورود و خروج خودرو (VACS) یک نرم‌افزار مدیریتی است که به منظور کنترل و نظارت بر تردد خودروها در محیط سازمانی طراحی شده است. هدف اصلی این سیستم افزایش امنیت سازمان از طریق کنترل دقیق ورود و خروج خودروهای مجاز و جلوگیری از تردد خودروهای غیرمجاز می‌باشد.

در این سازمان تعدادی راهبند وجود دارد که هر راهبند به یک یا چند دوربین پلاک‌خوان مجهز است. هنگامی که خودرویی به راهبند نزدیک می‌شود، دوربین پلاک‌خوان به‌صورت خودکار شماره پلاک خودرو را تشخیص داده و به موتور کنترل دسترسی ارسال می‌کند. سیستم پلاک دریافتی را با پایگاه داده تطبیق می‌دهد. در صورت وجود مجوز معتبر راهبند باز شده و رویداد با وضعیت GRANTED ثبت می‌گردد. در غیر این صورت راهبند بسته می‌ماند و رویداد با وضعیت DENIED ثبت می‌شود.



---
|## 💻 نمونه نرم‌افزار

🔗 **[اینجا کلیک کنید — نمونه نرم‌افزار آنلاین](https://khadijerokni.github.io/vehicle-access-control-system/software/VACS.html)**

فایل `software/VACS.html` را در مرورگر باز کنید.
هیچ نصبی لازم نیست.

| نقش | Username | Password |
|-----|----------|----------|
| Admin | admin | admin123 |
| Guard | guard1 | guard123 |

---


## 🎯 زیرسیستم‌ها

| زیرسیستم | توضیح |
|----------|-------|
| 🚗 تعریف خودرو | ثبت و مدیریت خودروها و مالکان |
| 🚧 تعریف راهبند | ثبت راهبندها و دوربین‌های پلاک‌خوان |
| 🔐 سطح دسترسی | تعریف مجوز دسترسی هر خودرو به راهبندها |
| 🚦 کنترل دسترسی | تشخیص پلاک و کنترل راهبند |
| 📋 لاگ تردد | ثبت رویدادهای ورود و خروج |
| 📈 گزارش‌دهی | مشاهده و خروجی CSV |

---

## 🏗️ معماری نرم‌افزار

**معماری: 3-Tier Architecture + MVC**

| لایه | مسئولیت |
|------|---------|
| Presentation Layer | رابط کاربری و Controllers |
| Business Logic Layer | Services و AccessControlEngine |
| Data Access Layer | Repositories |
| Database | SQLite |

---

## 📊 نمودارها

| نمودار | پوشه |
|--------|------|
| Use Case Diagram | diagrams/usecase/ |
| DFD Level 0 | diagrams/dfd/ |
| DFD Level 1 | diagrams/dfd/ |
| Class Diagram تحلیل | diagrams/class/ |
| Class Diagram طراحی | diagrams/class/ |
| Sequence Diagram 1 — ثبت خودرو | diagrams/sequence/ |
| Sequence Diagram 2 — اعطای مجوز | diagrams/sequence/ |
| Sequence Diagram 3 — ورود خودرو | diagrams/sequence/ |
| ERD — Chen Notation | diagrams/erd/ |
| Component Diagram | diagrams/component/ |
| Product Backlog | diagrams/backlog/ |

---

## ✅ چک‌لیست مستندات

- [x] شرح سیستم
- [x] نمودار Use Case
- [x] جدول Product Backlog — 24 User Story
- [x] نمودار کلاس تحلیل
- [x] DFD سطح ۰
- [x] DFD سطح ۱
- [x] نمودار توالی ۱ — ثبت خودرو
- [x] نمودار توالی ۲ — اعطای مجوز
- [x] نمودار توالی ۳ — ورود خودرو
- [x] نمودار ERD
- [x] معماری نرم‌افزار
- [x] نمودار کلاس طراحی
- [x] نمودار کامپوننت
- [x] نمونه نرم‌افزار
