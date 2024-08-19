[Vietnamese Version](./README.md)

## Introduction

**Optimal-Assets-Folder-Management** was created to propose an optimal folder structure for managing asset files in web projects. The goal of this project is to help developers easily manage, maintain, and scale interface files such as CSS, JavaScript, images, and third-party libraries in a logical and efficient manner.

## Motivation For The Project

In the process of web application development, maintaining a clear and organized folder structure is crucial. A reasonable folder structure not only improves work efficiency but also helps team members easily understand and approach the project. However, developers cannot always create an optimal structure from the start on their own.

This project was created to address that issue. It provides a standardized folder structure that can be easily applied to new or existing web projects. With clear separation between different types of assets and flexibility for expansion, I believe this project will help developers save time and effort while improving the quality of the web applications they build.

## Usage

Install.

```bash
npm install oafm 
```

## 📖 Directory Structure of Assets

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

### DEMO

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

## Contributions

If you would like to contribute to the project, please open a [pull request](https://github.com/HHiepz/Optimal-Assets-Folder-Management/pulls) or create an issue on GitHub. Any feedback is highly appreciated and will help improve the project.