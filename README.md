[English Version](./README_en.md)

## Giới Thiệu

**Optimal-Assets-Folder-Management** được tạo ra để đề xuất một cấu trúc thư mục **tối ưu việc quản lý các tệp tài nguyên (assets)** trong các dự án web. Mục tiêu của dự án là giúp các nhà phát triển dễ dàng quản lý, bảo trì và mở rộng các tệp giao diện như CSS, JavaScript, hình ảnh và các thư viện bên thứ ba một cách hợp lý và hiệu quả.

## Động Lực Tạo Ra Dự Án

Trong quá trình phát triển ứng dụng web, việc duy trì một cấu trúc thư mục rõ ràng và có tổ chức là rất quan trọng. Một cấu trúc thư mục hợp lý không chỉ giúp tăng hiệu suất làm việc mà còn giúp các thành viên trong nhóm dễ dàng hiểu và tiếp cận dự án. Tuy nhiên, không phải lúc nào các nhà phát triển cũng có thể tự mình xây dựng một cấu trúc tối ưu từ đầu.

Dự án này được tạo ra để giải quyết vấn đề đó. Nó cung cấp một cấu trúc thư mục chuẩn mực, dễ dàng áp dụng vào các dự án web mới hoặc hiện tại. Với sự phân tách rõ ràng giữa các loại tài nguyên và sự linh hoạt trong việc mở rộng, tôi tin rằng dự án này sẽ giúp các nhà phát triển tiết kiệm thời gian và nỗ lực, đồng thời nâng cao chất lượng của các ứng dụng web mà họ xây dựng.

## Khởi Tạo

Đối với bạn sử dụng VSCode, mở Terminal và chạy dòng lệnh sau sẽ tự render ra folder.

```bash
mkdir -p assets/css/components
mkdir -p assets/css/custom
mkdir -p assets/css/pages
mkdir -p assets/css/variables
mkdir -p assets/fonts
mkdir -p assets/images/logo
mkdir -p assets/images/icons
mkdir -p assets/images/backgrounds
mkdir -p assets/js/components
mkdir -p assets/js/custom
mkdir -p assets/js/pages
mkdir -p assets/vendors/bootstrap
mkdir -p assets/vendors/datatables
mkdir -p assets/vendors/jquery
```


## 📖 Bố Cục Thư Mục Assets

```yaml
assets
├─ css
│  ├─ components
│  ├─ custom
│  ├─ pages
│  ├─ variables
│
├─ fonts
│
├─ images
│  ├─ logo
│  ├─ icons
│  ├─ backgrounds
│
├─ js
│  ├─ components
│  ├─ custom
│  ├─ pages
│
├─ vendors
│  ├─ bootstrap
│  ├─ datatables
│  ├─ jquery
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

### DEMO

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
    <!-- Custom CSS for page -->
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
    <!-- Custom JS for page -->
    <script src="assets/js/pages/page-index.js"></script>
    <script src="assets/js/pages/page-profile.js"></script>
</body>

</html>
```

## Đóng Góp

Nếu bạn muốn đóng góp vào dự án, hãy mở [pull request](https://github.com/HHiepz/Optimal-Assets-Folder-Management/pulls) hoặc tạo issue trên GitHub. Mọi ý kiến đóng góp đều rất đáng quý và sẽ giúp cải thiện dự án.
