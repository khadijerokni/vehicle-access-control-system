# DFD — Data Flow Diagram

استاندارد: Yourdon-DeMarco

## سطح ۰ — Context Diagram

کل سیستم به صورت یک پروسه واحد نشان داده شده است.

### موجودیت‌های خارجی

| موجودیت | ورودی به سیستم | خروجی از سیستم |
|---------|--------------|----------------|
| Admin | اطلاعات خودرو، راهبند، مجوز | تاییدیه، گزارش |
| Vehicle / Driver | پلاک خودرو | نتیجه دسترسی |
| Barrier / Camera | تصویر پلاک | دستور باز/بسته |
| Security Guard | Override دستی | لاگ رویدادها |
| Report Consumer | — | گزارش تردد |

## سطح ۱ — Detailed DFD

### پروسه‌ها

| شماره | نام | توضیح |
|-------|-----|-------|
| 1.1 | Manage Vehicle | مدیریت خودروها و مالکان |
| 1.2 | Manage Barrier | مدیریت راهبندها و دوربین‌ها |
| 1.3 | Manage Access Permission | مدیریت مجوزهای دسترسی |
| 1.4 | Detect & Control | تشخیص پلاک و کنترل راهبند |
| 1.5 | Log Event | ثبت رویدادهای تردد |
| 1.6 | Generate Report | تولید گزارش |

### Data Store‌ها

| Data Store | محتوا |
|-----------|-------|
| D1 Vehicles | اطلاعات خودروها |
| D2 Owners | اطلاعات مالکان |
| D3 Barriers | اطلاعات راهبندها |
| D4 Cameras | اطلاعات دوربین‌ها |
| D5 Access Permissions | مجوزهای دسترسی |
| D6 Access Log | لاگ رویدادها |

## فایل‌ها
- `dfd_level0.png` — DFD سطح ۰
- `dfd_level1.png` — DFD سطح ۱
