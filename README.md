/* Thanh điều hướng */
        nav { 
            grid-area: nav; 
            background: var(--mau-phu); 
            /* Bỏ padding ở đây để nhường padding cho thẻ a */
        }
        
        nav ul { 
            list-style: none; 
            margin: 0; 
            padding: 0; 
            display: flex; 
            justify-content: center; /* Căn giữa theo chiều ngang */
            align-items: center;     /* Căn giữa tuyệt đối theo chiều dọc */
            min-height: 50px;        /* Chiều cao tối thiểu của thanh menu */
            gap: 10px; 
        }
        
        nav a { 
            color: white; 
            text-decoration: none; 
            font-weight: bold; 
            text-transform: uppercase; 
            display: flex;           /* Biến thẻ a thành khối linh hoạt */
            align-items: center;     /* Căn giữa chữ bên trong thẻ a */
            padding: 10px 20px;      /* Mở rộng vùng bấm chuột (trên/dưới 10px, trái/phải 20px) */
            border-radius: 4px;      /* Bo góc một chút cho đẹp */
            transition: background 0.3s; /* Hiệu ứng chuyển màu mượt mà */
        }

        /* Thêm hiệu ứng khi di chuột (hover) vào menu */
        nav a:hover {
            background-color: var(--mau-chinh);
        }
