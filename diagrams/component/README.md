# Component Diagram | نمودار کامپوننت

## توضیح
نمودار کامپوننت اجزای اصلی سیستم و وابستگی‌ها را نشان می‌دهد.

## کامپوننت‌ها

### Client — Browser
- Dashboard UI
- Vehicle Management UI
- Barrier Management UI
- Permission Management UI
- Access Control UI
- Log & Report UI

### Application Server
- Router / Controller
- VehicleService
- BarrierService
- AccessPermissionService
- AccessControlEngine
- ReportService
- AuthService
- VehicleRepository
- BarrierRepository
- PermissionRepository
- LogRepository
- CameraRepository
- OperatorRepository

### Data Storage
- SQLite Database
  - owner
  - vehicle
  - barrier
  - camera
  - access_permission
  - access_log
  - operator

### Physical Hardware
- Plate Reader Camera
- Barrier Motor Controller

## جریان داده

###فایل ها 

component _diagram.png
