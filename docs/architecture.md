# معماری نرم‌افزار | Software Architecture

## معماری انتخابی: 3-Tier Architecture + MVC

### لایه‌ها

| لایه | مسئولیت | کامپوننت‌ها |
|------|---------|------------|
| Presentation Layer | رابط کاربری | Controllers |
| Business Logic Layer | قوانین کسب‌وکار | Services, AccessControlEngine |
| Data Access Layer | دسترسی به داده | Repositories |
| Database | ذخیره داده | SQLite |

### دلایل انتخاب
- Separation of Concerns — جداسازی مسئولیت‌ها
- قابلیت توسعه و نگهداری آسان
- استقلال لایه‌ها از یکدیگر
- مناسب سیستم‌های سازمانی

### Design Patterns
- **MVC** برای لایه نمایش
- **Repository Pattern** برای دسترسی به داده
- **Service Layer** برای منطق کسب‌وکار

### کامپوننت‌های Business Logic
| کامپوننت | وظیفه |
|---------|-------|
| VehicleService | مدیریت خودروها |
| BarrierService | مدیریت راهبندها |
| AccessPermissionService | مدیریت مجوزها |
| AccessControlEngine | تشخیص پلاک و کنترل راهبند |
| ReportService | گزارش‌دهی |
| AuthService | احراز هویت |
