# Sequence Diagrams | نمودارهای توالی

## SD-1 — ثبت خودرو جدید

**سناریو:** Admin یک خودرو جدید ثبت می‌کند

**مطابق Backlog:** US-01, US-05

**مراحل:**
1. Admin فرم ثبت خودرو را باز می‌کند
2. سیستم لیست مالکان را نمایش می‌دهد
3. Admin اطلاعات را وارد می‌کند
4. سیستم پلاک را بررسی می‌کند
5. خودرو در پایگاه داده ذخیره می‌شود

**مطابق با:** VehicleController, VehicleService, VehicleRepository, VEHICLE در ERD, پروسه ۱.۱ در DFD

---

## SD-2 — اعطای مجوز دسترسی

**سناریو:** Admin به خودرو مجوز دسترسی می‌دهد

**مطابق Backlog:** US-11, US-12, US-13

**مراحل:**
1. Admin فرم مجوز را باز می‌کند
2. سیستم لیست خودروها و راهبندها را نمایش می‌دهد
3. Admin خودرو، راهبند، جهت و بازه زمانی را انتخاب می‌کند
4. سیستم مجوز تکراری را بررسی می‌کند
5. مجوز ذخیره می‌شود

**مطابق با:** PermissionController, AccessPermissionService, PermissionRepository, ACCESS_PERMISSION در ERD, پروسه ۱.۳ در DFD

---

## SD-3 — ورود خودرو به سازمان

**سناریو:** خودرو به راهبند نزدیک می‌شود

**مطابق Backlog:** US-16, US-17, US-18, US-19

**مراحل:**
1. خودرو به راهبند نزدیک می‌شود
2. دوربین پلاک را تشخیص می‌دهد
3. سیستم خودرو را جستجو می‌کند
4. سیستم مجوز فعال را بررسی می‌کند
5. بازه زمانی و ساعت بررسی می‌شود
6. راهبند باز یا بسته می‌ماند
7. رویداد در لاگ ثبت می‌شود

**مطابق با:** AccessControlEngine, VehicleRepository, PermissionRepository, LogRepository, ACCESS_LOG در ERD, پروسه ۱.۴ و ۱.۵ در DFD

## فایل‌ها
- `sd1_register_vehicle.png`
- `sd2_grant_permission.png`
- `sd3_vehicle_entry.png`
