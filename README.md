## 📖 Bố Cục Thư Mục Assets

[English Version](README_en.md)

```
assets
├─ css
│  ├─ components
│  │  ├─ table.css
│  │  ├─ button.css
│  │  └─ ...
│  ├─ custom
│  │  ├─ custom-datatables.css
│  │  ├─ custom-bootstrap.css
│  │  └─ ...
│  ├─ pages
│  │  ├─ page-index.css
│  │  ├─ page-profile.css
│  │  └─ ...
│  ├─ variables
│  │  ├─ colors.css
│  │  └─ ...
│
├─ fonts
│  └─ ...
│
├─ images
│  ├─ logo
│  │  └─ logo.png
│  ├─ icons
│  │  └─ icon.svg
│  ├─ backgrounds
│  │  └─ bg.jpg
│  └─ ...
│
├─ js
│  ├─ components
│  │  ├─ table.js
│  │  ├─ button.js
│  │  └─ ...
│  ├─ custom
│  │  ├─ custom-datatables.js
│  │  ├─ custom-bootstrap.js
│  │  └─ ...
│  ├─ pages
│  │  ├─ page-profile.js
│  │  └─ ...
│
├─ vendors
│  ├─ bootstrap
│  │  ├─ bootstrap-5.1.3.min.css
│  │  ├─ bootstrap.bundle-5.1.3.js
│  │  └─ ...
│  ├─ datatables
│  │  ├─ datatables.min.css
│  │  ├─ datatables.min.js
│  │  └─ ...
│  ├─ jquery
│  │  ├─ jquery.min-3.7.1.js
│  │  └─ ...
│  └─ ...
```

## 📋 Giải Thích Chi Tiết Bố Cục

**assets**: Chứa tất cả nội dung tĩnh cho dự án, bao gồm biểu định kiểu, tệp JavaScript, hình ảnh và phông chữ.

- **`css`**: Chứa toàn bộ file CSS.
  - **`components`**: Tùy chỉnh riêng cho từng thành phần dùng chung trong dự án.
  - **`custom`**: Tùy chỉnh lại thiết kế của thư viện và plugins.
  - **`pages`**: Tùy chỉnh các kiểu thiết kế dùng riêng cho mỗi trang.
  - **`varibles`**: Tùy chỉnh biến, ví dụ: `colorText`, `colorBorder`, `colorBackground`,..

- **`js`**: Chứa toàn bộ file JavaScript.
  - **`components`**: Tùy chỉnh riêng cho từng thành phần dùng chung trong dự án.
  - **`custom`**: Tùy chỉnh lại các thư viện và plugins.
  - **`pages`**: Tùy chỉnh các script dùng riêng cho mỗi trang.

- **`vendors`**: Chứa toàn bộ thư viện bên thứ ba (frameworks).
  - **`library-name`**: Mỗi thư viện/framework có một thư mục riêng, ví dụ: `bootstrap`, `datatables`, `jquery`.

- **`fonts`**: Chứa toàn bộ file phông chữ.

- **`images`**: Chứa toàn bộ hình ảnh.
  - **`image-name`**: Mỗi phần có mỗi thư mục riêng, ví dụ: `icons`, `logo`, `backgrounds`, `products`,..

### Sử Dụng

Để sử dụng dự án, bao gồm các file CSS và JS cần thiết trong file HTML của bạn. Dưới đây là một ví dụ:

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <!-- Fonts -->
    <link rel="stylesheet" href="assets/fonts/...">
    <!-- Vendor CSS -->
    <link rel="stylesheet" href="assets/vendors/bootstrap/bootstrap.min-5.3.3.css">
    <link rel="stylesheet" href="assets/vendors/datatable/dataTables.min.css">
    <!-- Custom CSS -->
    <link rel="stylesheet" href="assets/css/custom/custom-bootstrap.css">
    <link rel="stylesheet" href="assets/css/custom/custom-datatables.css">
    <!-- Custom CSS for profile page -->
    <link rel="stylesheet" href="assets/css/pages/page-index.css">
    <link rel="stylesheet" href="assets/css/pages/page-profile.css">
</head>

<body>

    <!-- Example button using custom Bootstrap styles -->
    <button class="btn btn-custom">Custom Button</button>

    <!-- Example DataTable -->
    <div class="container">
        <table id="example" class="display" style="width:100%">
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Position</th>
                    <th>Office</th>
                    <th>Age</th>
                    <th>Start date</th>
                    <th>Salary</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Tiger Nixon</td>
                    <td>System Architect</td>
                    <td>Edinburgh</td>
                    <td>61</td>
                    <td>2011/04/25</td>
                    <td>$320,800</td>
                </tr>
                <!-- More rows here -->
            </tbody>
        </table>
    </div>

    <!-- Vendor JS -->
    <script src="assets/vendors/jquery/jquery.min-3.7.1.js"></script>
    <script src="assets/vendors/bootstrap/bootstrap.bundle-5.3.3.js"></script>
    <script src="assets/vendors/datatable/dataTables.min.js"></script>
    <!-- Custom JS -->
    <script src="assets/js/custom/custom-bootstrap.js"></script>
    <script src="assets/js/custom/custom-datatables.js"></script>
    <!-- Custom JS for profile page -->
    <script src="assets/js/pages/page-index.js"></script>
    <script src="assets/js/pages/page-profile.js"></script>
</body>

</html>
```