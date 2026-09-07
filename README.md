<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Một trang web HTML nâng cao với CSS và JavaScript">
    <title>Trang Web Nâng Cao</title>
    
    <!-- Phần CSS dùng để trang trí giao diện (Style) -->
    <style>
        /* Sử dụng biến CSS */
        :root {
            --mau-chinh: #2c3e50;
            --mau-phu: #3498db;
        }

        /* Thiết lập bố cục (Layout) sử dụng CSS Grid */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            display: grid;
            grid-template-areas:
                "header header"
                "nav nav"
                "main sidebar"
                "footer footer";
            grid-template-columns: 3fr 1fr;
            min-height: 100vh;
            background-color: #f9f9f9;
        }

        header { grid-area: header; background: var(--mau-chinh); color: white; padding: 20px; text-align: center; }
        nav { grid-area: nav; background: var(--mau-phu); padding: 10px; }
        nav ul { list-style: none; margin: 0; padding: 0; display: flex; justify-content: center; gap: 20px; }
        nav a { color: white; text-decoration: none; font-weight: bold; text-transform: uppercase; }
        main { grid-area: main; padding: 20px; }
        aside { grid-area: sidebar; background: #e0e0e0; padding: 20px; border-left: 2px solid #ccc; }
        footer { grid-area: footer; background: #222; color: white; text-align: center; padding: 15px; }

        /* Trang trí cho khối nội dung (Card) */
        .card {
            background: white;
            border-radius: 8px;
            padding: 20px;
            margin-bottom: 20px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }

        /* Trang trí cho bảng (Table) */
        table { width: 100%; border-collapse: collapse; margin-top: 15px; }
        th, td { border: 1px solid #ddd; padding: 10px; text-align: left; }
        th { background-color: var(--mau-phu); color: white; }

        /* Trang trí nút bấm */
        button {
            background-color: var(--mau-phu);
            color: white;
            border: none;
            padding: 10px 15px;
            cursor: pointer;
            border-radius: 4px;
        }
        button:hover { background-color: var(--mau-chinh); }
    </style>
</head>
<body>

    <!-- Phần Tiêu đề trang -->
    <header>
        <h1>Hệ Thống Quản Lý Giao Diện Nâng Cao</h1>
        <p>Ví dụ về cấu trúc HTML5 ngữ nghĩa, CSS Grid và JavaScript</p>
    </header>

    <!-- Thanh Điều hướng -->
    <nav>
        <ul>
            <li><a href="#home">Trang chủ</a></li>
            <li><a href="#services">Dịch vụ</a></li>
            <li><a href="#contact">Liên hệ</a></li>
        </ul>
    </nav>

    <!-- Khu vực nội dung chính -->
    <main>
        <section id="home">
            <h2>Nội dung chính của trang</h2>
            
            <article class="card">
                <h3>Bài viết tương tác</h3>
                <p>Đây là một thẻ <code>&lt;article&gt;</code> chứa đoạn văn bản. Nhấn vào nút bên dưới để gọi lệnh JavaScript.</p>
                <button onclick="hienThongBao()">Nhấn vào tôi!</button>
            </article>

            <article class="card">
                <h3>Bảng Dữ Liệu Nhân Viên</h3>
                <table>
                    <thead>
                        <tr>
                            <th>ID</th>
                            <th>Họ và Tên</th>
                            <th>Chức vụ</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>NV01</td>
                            <td>Nguyễn Văn A</td>
                            <td>Quản trị viên</td>
                        </tr>
                        <tr>
                            <td>NV02</td>
                            <td>Trần Thị B</td>
                            <td>Nhân viên</td>
                        </tr>
                    </tbody>
                </table>
            </article>
        </section>
    </main>

    <!-- Thanh bên (Sidebar) -->
    <aside>
        <h3>Đăng ký nhận tin</h3>
        <p>Điền form dưới đây để nhận thông báo mới nhất.</p>
        <!-- Biểu mẫu (Form) -->
        <form action="#" method="POST">
            <label for="email">Email của bạn:</label><br>
            <input type="email" id="email" name="email" placeholder="example@gmail.com" required style="width: 90%; margin: 10px 0; padding: 8px;"><br>
            <button type="submit">Gửi thông tin</button>
        </form>
    </aside>

    <!-- Chân trang -->
    <footer>
        <p>&copy; 2026 Bản quyền thuộc về Bạn. Thiết kế bởi HTML/CSS.</p>
    </footer>

    <!-- Phần JavaScript dùng để xử lý logic -->
    <script>
        function hienThongBao() {
            alert("Tuyệt vời! JavaScript đang hoạt động. Mã HTML này nhìn có vẻ phức tạp nhưng thực ra rất logic.");
        }
    </script>

</body>
</html>
