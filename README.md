## 🙋‍♂️ Ghi chú từ tác giả
Đây là dự án nhóm trong quá trình học tập/thực hành.  
Mặc dù không phải là dự án cá nhân, nhưng tôi đã nỗ lực hết sức trong phần việc của mình, chủ động tìm hiểu và đóng góp để hoàn thành dự án.  
Tôi hy vọng dự án này sẽ thể hiện tinh thần học hỏi, khả năng làm việc nhóm cũng như sự cam kết của tôi trong công việc.

# 💄 SellingCosmetics

## 📌 Tổng quan
**SellingCosmetics** là một ứng dụng web dùng để quản lý và bán các sản phẩm mỹ phẩm.  
Dự án được phát triển bằng **ASP.NET MVC** theo kiến trúc **Model-View-Controller (MVC)**, cung cấp các chức năng như quản lý sản phẩm, giỏ hàng, khuyến mãi và báo cáo.


---
## 🚀 Features

- 🔍 **Tìm kiếm & lọc sản phẩm** theo tên, loại, thương hiệu
- 🛒 **Giỏ hàng** (thêm, sửa, xóa sản phẩm)
- 💳 **Thanh toán** và quản lý đơn hàng
- 👤 **Quản lý người dùng** (đăng ký, đăng nhập, phân quyền)
- ⭐ **Đánh giá & khuyến mãi**
- 📊 **Quản trị hệ thống** (thêm, sửa, xóa sản phẩm, xem báo cáo)

---

## 🏗 Project Structure

```text
📂 DOAN/                          # Main ASP.NET MVC project
├── 📂 App_Start/                 # MVC configuration files (RouteConfig, FilterConfig, etc.)
├── 📂 Common/                    # Common utilities and helpers
├── 📂 Content/                   # CSS and static files
├── 📂 Controllers/               # MVC Controllers (handle requests and business logic)
│   ├── 📄 DashboardController.cs
│   ├── 📄 DeliveryController.cs
│   ├── 📄 CartController.cs
│   ├── 📄 HomeController.cs
│   ├── 📄 UserController.cs
│   ├── 📄 ImportController.cs
│   ├── 📄 InvoiceController.cs
│   ├── 📄 PromotionController.cs
│   ├── 📄 CategoryController.cs
│   ├── 📄 ProductController.cs
│   └── 📄 SearchController.cs
│
├── 📂 Models/                    # Data models (Entity Framework classes)
│   ├── 📄 InvoiceDetail.cs
│   ├── 📄 Cart.cs
│   ├── 📄 Invoice.cs
│   ├── 📄 Promotion.cs
│   ├── 📄 Category.cs
│   ├── 📄 User.cs
│   ├── 📄 Product.cs
│   ├── 📄 Brand.cs
│   ├── 📄 Role.cs
│   ├── 📄 Import.cs
│   └── 📄 TMDTDbContext.cs       # Database context
│
├── 📂 Views/                     # Razor views for UI
│   ├── 📂 Dashboard/
│   ├── 📂 Cart/
│   ├── 📂 Home/
│   ├── 📂 User/
│   ├── 📂 Import/
│   ├── 📂 Invoice/
│   ├── 📂 Promotion/
│   ├── 📂 Category/
│   ├── 📂 Product/
│   ├── 📂 Brand/
│   └── 📂 Shared/                # Layout and partial views
│
├── 📂 Scripts/                   # JavaScript files
├── 📂 assets/                    # Static resources (images, fonts, etc.)
├── 📂 csdl moi/                  # Database backup (.bak)
├── 📂 packages/                  # NuGet packages
├── 📄 DOAN.sln                   # Visual Studio solution file
└── 📄 Web.config                 # Application configuration
```
---
## 🚀 Installation & Setup
1. **Clone the repository**
   git clone https://github.com/Mit2611/SellingCosmetics.git
2. **Open the solutio**
Open DOAN.sln in Visual Studio.
3. **Restore NuGet packages**
Visual Studio will auto-restore, or run:
Update-Package -reinstall
4. **Configure Database Connection**
Edit the connection string in Web.config to match your local SQL Server instance.
5. **Database Setup**  
   - Option 1: Run Entity Framework migrations.  
   - Option 2: Restore database from `csdl moi/TMDTM.bak`.

6. **Run the Project**
Press F5 in Visual Studio to start debugging.
