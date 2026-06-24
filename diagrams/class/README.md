# Class Diagrams | نمودارهای کلاس

## فاز تحلیل (Analysis)

موجودیت‌های اصلی سیستم و روابط بین آنها.

### کلاس‌های اصلی

| کلاس | توضیح | کلید اصلی |
|------|-------|-----------|
| Owner | مالک / پرسنل | owner_id |
| Vehicle | خودرو | vehicle_id |
| Barrier | راهبند | barrier_id |
| Camera | دوربین پلاک‌خوان | camera_id |
| AccessPermission | مجوز دسترسی | permission_id |
| AccessLog | لاگ رویداد | log_id |
| Operator | کاربر سیستم | operator_id |

### روابط
- Owner 1 به N Vehicle
- Vehicle 1 به N AccessPermission
- Barrier 1 به N AccessPermission
- Barrier 1 به N Camera
- AccessPermission 1 به N AccessLog

## فاز طراحی (Design)

معماری سه‌لایه کامل.

### لایه‌ها

| لایه | کلاس‌ها |
|------|---------|
| Presentation | DashboardController, VehicleController, BarrierController, PermissionController, AccessControlController, LogController, AuthController |
| Business Logic | VehicleService, BarrierService, AccessPermissionService, AccessControlEngine, ReportService, AuthService |
| Data Access | VehicleRepository, BarrierRepository, PermissionRepository, LogRepository, CameraRepository, OperatorRepository |
| Domain | Owner, Vehicle, Barrier, Camera, AccessPermission, AccessLog, Operator |

## فایل‌ها
- `class_analysis.png` — نمودار کلاس تحلیل
- `class_design.png` — نمودار کلاس طراحی
