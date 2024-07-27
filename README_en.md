## 📖 Directory Structure of Assets

[Vietnamese Version](README.md)

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

## 📋 Detailed Directory Explanation

**assets**: Contains all static content for the project, including stylesheets, JavaScript files, images, and fonts.

- **`css`**: Contains all CSS files.
  - **`components`**: Custom styles for individual reusable components in the project..
  - **`custom`**: Customizations of third-party libraries and plugins.
  - **`pages`**: Custom styles specific to each page.
  - **`varibles`**: CSS variables, e.g., `colorText`, `colorBorder`, `colorBackground`, etc

- **`js`**: Contains all JavaScript files.
  - **`components`**: Custom scripts for individual reusable components in the project.
  - **`custom`**: Customizations of third-party libraries and plugins.
  - **`pages`**: Custom scripts specific to each page.

- **`vendors`**: Contains all third-party libraries (frameworks).
  - **`library-name`**: Each library/framework has its own directory, e.g., `bootstrap`, `datatables`, `jquery`, etc.

- **`fonts`**: Contains all font files.

- **`images`**: Contains all images.
  - **`image-name`**: Each category has its own directory, e.g.,`icons`, `logo`, `backgrounds`, `products`, etc.

### Usage

To use the project, include the necessary CSS and JS files in your HTML file. Here is an example:

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