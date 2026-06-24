# Use Case Diagram

## توضیح
نمودار Use Case تمام تعاملات بین کاربران و سیستم را نشان می‌دهد.

## بازیگران

| Actor | نقش |
|-------|-----|
| Admin | مدیریت کامل سیستم |
| Security Guard | مشاهده لاگ و کنترل دستی |
| Driver / Vehicle | تردد از راهبند |
| Barrier / Camera | تشخیص پلاک خودکار |

## پکیج‌ها و Use Case‌ها

| پکیج | Use Case‌ها |
|------|------------|
| Vehicle Management | Register Vehicle, Edit Vehicle, Deactivate Vehicle, Register Owner, View List |
| Barrier Management | Register Barrier, Edit Barrier, Deactivate Barrier, Assign Camera, View List |
| Access Permission | Grant Permission, Set Time Range, Set Direction, Revoke, View |
| Core | Detect Plate, Check Permission, Open/Close Barrier, Log Event, Deny |
| Reports | View Logs, Filter Logs, Export Report |
| Authentication | Login, Manage Operators |

## روابط
- Admin به تمام Use Case‌های مدیریتی دسترسی دارد
- Guard به لاگ و کنترل دستی دسترسی دارد
- Camera/Driver به Core Use Case‌ها مرتبط است
- رابطه include بین Detect Plate و Check Permission
- رابطه include بین Check Permission و Open/Close Barrier

## فایل
- `usecase_diagram.png`
