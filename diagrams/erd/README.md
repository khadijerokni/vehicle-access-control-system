# ERD — Entity Relationship Diagram

سبک: Chen Notation

## نمادها

| نماد | معنی |
|------|------|
| مستطیل | موجودیت Entity |
| بیضی | صفت Attribute |
| بیضی با خط زیر | کلید اصلی PK |
| لوزی | رابطه Relationship |
| 1 و N | ضریب ارتباط Cardinality |

## موجودیت‌ها

| موجودیت | کلید اصلی | صفات مهم |
|---------|-----------|---------|
| OWNER | owner_id | first_name, last_name, national_id, department |
| VEHICLE | vehicle_id | plate_number, brand, model, color, vehicle_type |
| BARRIER | barrier_id | barrier_name, location, direction, status |
| CAMERA | camera_id | ip_address, model, status |
| ACCESS_PERMISSION | permission_id | access_type, valid_from, valid_until, time_from, time_until |
| ACCESS_LOG | log_id | event_type, event_datetime, detected_plate, access_status |
| OPERATOR | operator_id | username, role |

## روابط

| رابطه | موجودیت‌ها | نوع |
|-------|-----------|-----|
| owns | OWNER — VEHICLE | 1:N |
| has_permission | VEHICLE — ACCESS_PERMISSION | 1:N |
| controls | BARRIER — ACCESS_PERMISSION | 1:N |
| has_camera | BARRIER — CAMERA | 1:N |
| logs | ACCESS_PERMISSION — ACCESS_LOG | 1:N |
| manages | OPERATOR — ACCESS_LOG | 1:N |

## فایل‌ها
- `erd_chen.png` — تصویر ERD
- `erd_chen.drawio` — فایل قابل ویرایش
