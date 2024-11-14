<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>متجر الألبسة والمنتجات</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f4f4f4;
        }
        nav {
            margin: 20px;
        }
        nav a {
            margin: 15px;
            text-decoration: none;
            color: #007BFF;
        }
        .tab {
            display: none;
        }
        .active {
            display: block;
        }
    </style>
</head>
<body>
    <h1>مرحبا بكم في موقع سبوس دلندح</h1>
    <nav>
        <a href="#" onclick="showTab('home')">الرئيسية</a>
        <a href="#" onclick="showTab('clothes')">الألبسة</a>
        <a href="#" onclick="showTab('products')">المنتجات</a>
    </nav>

    <div id="home" class="tab active">
        <p>استمتع بتصفح منتجاتنا المميزة!</p>
    </div>

    <div id="clothes" class="tab">
        <h2>قسم الألبسة</h2>
        <p>نقدم مجموعة متنوعة من الألبسة العصرية.</p>
        <ul>
            <li>تي شيرتات</li>
            <li>سراويل</li>
            <li>فساتين</li>
            <li>معاطف</li>
        </ul>
    </div>

    <div id="products" class="tab">
        <h2>قسم المنتجات</h2>
        <p>اكتشف منتجاتنا الرائعة!</p>
        <ul>
            <li>منتج 1</li>
            <li>منتج 2</li>
            <li>منتج 3</li>
            <li>منتج 4</li>
        </ul>
    </div>

    <script>
        function showTab(tabId) {
            const tabs = document.querySelectorAll('.tab');
            tabs.forEach(tab => {
                tab.classList.remove('active');
            });
            document.getElementById(tabId).classList.add('active');
        }
    </script>
</body>
</html>