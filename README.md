<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lồng Đèn Hạnh Đào - Xưởng Sản Xuất Đèn Lồng Hội An | longdenhanhdao.com</title>
  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- Font Awesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
  <!-- Google Fonts: Inter & Playfair Display (Chuẩn phong cách truyền thống kết hợp hiện đại dễ dùng trên Flatsome) -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Playfair+Display:wght@600;700&display=swap" rel="stylesheet">

  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            brand: {
              red: '#9E1B1B',      // Đỏ trầm truyền thống Hội An
              darkRed: '#7A1212',  // Đỏ đậm
              gold: '#D4AF37',     // Vàng đồng ấm
              lightGold: '#FDF8E7',// Nền kem vàng nhạt
              bg: '#FAF7F2'        // Nền trang kem sáng nhẹ chuẩn Flatsome
            }
          },
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
            serif: ['Playfair Display', 'serif']
          }
        }
      }
    }
  </script>

  <style>
    body {
      font-family: 'Inter', sans-serif;
      background-color: #FAF7F2;
      color: #262626;
      overflow-x: hidden;
    }

    /* Chuẩn khung Container 1200px của Flatsome */
    .flatsome-container {
      max-width: 1200px;
      margin-left: auto;
      margin-right: auto;
      padding-left: 15px;
      padding-right: 15px;
    }

    /* Tiêu đề Section kiểu Flatsome [title style="center"] */
    .section-title-container {
      display: flex;
      align-items: center;
      justify-content: center;
      margin-bottom: 1.5rem;
    }
    .section-title-line {
      flex: 1;
      height: 2px;
      background-color: #e5dcd0;
    }
    .section-title-text {
      padding: 0 1.25rem;
      font-weight: 700;
      text-transform: uppercase;
      color: #9E1B1B;
      letter-spacing: 0.04em;
      text-align: center;
    }

    /* Hiệu ứng mượt cho ảnh sản phẩm chuẩn Flatsome image-zoom */
    .box-image {
      overflow: hidden;
      position: relative;
    }
    .box-image img {
      transition: transform 0.45s cubic-bezier(0.25, 0.46, 0.45, 0.94);
    }
    .product-box:hover .box-image img,
    .cat-box:hover .box-image img {
      transform: scale(1.06);
    }

    /* Hiệu ứng sóng lan tỏa cho nút liên hệ nổi */
    @keyframes pulse-ring {
      0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(220, 38, 38, 0.7); }
      70% { transform: scale(1); box-shadow: 0 0 0 12px rgba(220, 38, 38, 0); }
      100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(220, 38, 38, 0); }
    }
    @keyframes pulse-zalo {
      0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(0, 104, 255, 0.7); }
      70% { transform: scale(1); box-shadow: 0 0 0 12px rgba(0, 104, 255, 0); }
      100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(0, 104, 255, 0); }
    }
    .animate-pulse-red {
      animation: pulse-ring 2s infinite;
    }
    .animate-pulse-blue {
      animation: pulse-zalo 2s infinite;
    }

    /* Ẩn thanh cuộn ngang nhưng vẫn vuốt được */
    .no-scrollbar::-webkit-scrollbar {
      display: none;
    }
    .no-scrollbar {
      -ms-overflow-style: none;
      scrollbar-width: none;
    }

    /* Giới hạn 2 dòng tên sản phẩm để cột điện thoại luôn bằng nhau */
    .line-clamp-2 {
      display: -webkit-box;
      -webkit-line-clamp: 2;
      -webkit-box-orient: vertical;
      overflow: hidden;
    }
  </style>
</head>
<body class="antialiased selection:bg-brand-red selection:text-white">

  <!-- =========================================================
       1. FLATSOME TOP BAR (Chỉ hiển thị thông tin cửa hàng, không có thanh chỉnh sửa)
  ========================================================== -->
  <div class="bg-brand-darkRed text-amber-100 text-xs py-2 border-b border-red-900/60">
    <div class="flatsome-container flex flex-col sm:flex-row items-center justify-between gap-1.5">
      <div class="flex items-center gap-2 text-center sm:text-left">
        <i class="fa-solid fa-lantern text-brand-gold"></i>
        <span><strong>LỒNG ĐÈN HẠNH ĐÀO</strong> – Xưởng sản xuất đèn lồng Hội An sỉ & lẻ giá gốc | <strong>longdenhanhdao.com</strong></span>
      </div>
      <div class="flex flex-wrap items-center justify-center gap-4 text-xs">
        <a href="#ban-do-trang-chu" class="hover:text-white transition flex items-center gap-1">
          <i class="fa-solid fa-location-dot text-brand-gold"></i>
          <span>92 Nguyễn Du, Hội An, Đà Nẵng</span>
        </a>
        <span class="hidden md:inline text-red-400">|</span>
        <a href="tel:0796693304" class="hover:text-white transition flex items-center gap-1 font-semibold text-amber-200">
          <i class="fa-solid fa-phone-volume text-brand-gold"></i>
          <span>0796.693.304</span>
        </a>
      </div>
    </div>
  </div>

  <!-- =========================================================
       2. FLATSOME HEADER MAIN (Logo Fanpage + Tìm kiếm + Hotline)
  ========================================================== -->
  <header class="bg-white sticky top-0 z-40 shadow-sm border-b border-stone-200">
    <div class="flatsome-container py-3 md:py-4">
      <div class="flex items-center justify-between gap-3 md:gap-6">
        
        <!-- Nút mở Menu trên Điện thoại -->
        <button onclick="toggleMobileMenu()" aria-label="Mở danh mục" class="lg:hidden p-2.5 rounded-lg border border-stone-200 text-brand-red hover:bg-red-50 transition">
          <i class="fa-solid fa-bars text-xl"></i>
        </button>

        <!-- Logo Lồng Đèn Hạnh Đào (Đưa đúng mẫu Logo ảnh tròn nền đen "Cơ Sở Sản Xuất Lồng Đèn Hạnh Đào" vào trang web) -->
        <a href="#" onclick="filterByCategory('all'); return false;" class="flex items-center gap-3.5 group shrink-0">
          <div class="relative w-16 h-16 md:w-20 md:h-20 rounded-full border-2 border-[#D4AF37] overflow-hidden bg-[#0b0908] flex items-center justify-center shadow-lg shrink-0">
            <img 
              src="image_c19582.jpg" 
              alt="Logo Cơ Sở Sản Xuất Lồng Đèn Hạnh Đào Hội An" 
              class="w-full h-full object-cover"
              onerror="this.style.display='none'; document.getElementById('hanhdao-exact-logo').style.display='block';"
            >
            <!-- Bản hiển thị chính xác từng chi tiết của Logo ảnh Lồng Đèn Hạnh Đào (kèm nền đèn lồng Hội An, lồng đèn tre, Chùa Cầu, 5 icon, Zalo 0796 693 304) -->
            <div id="hanhdao-exact-logo" style="display:none;" class="w-full h-full relative bg-[#0b0908] select-none">
              <img 
                src="https://commons.wikimedia.org/wiki/Special:FilePath/Making_lanterns_in_Hoi_An_(31477021917).jpg?width=400" 
                alt="" 
                class="absolute inset-0 w-full h-full object-cover opacity-35"
              >
              <div class="absolute inset-0 bg-gradient-to-b from-black/80 via-black/65 to-black/90"></div>
              <svg class="relative z-10 w-full h-full" viewBox="0 0 240 240" fill="none" xmlns="http://www.w3.org/2000/svg">
                <!-- Viền tròn vàng đồng chuẩn mẫu -->
                <circle cx="120" cy="120" r="116" stroke="#E5C158" stroke-width="4"/>
                <circle cx="120" cy="120" r="111" stroke="#E5C158" stroke-width="1" stroke-opacity="0.45"/>

                <!-- Biểu tượng đèn lồng nét vẽ vàng ở đỉnh -->
                <ellipse cx="120" cy="27" rx="16" ry="13" stroke="#E5C158" stroke-width="1.6"/>
                <ellipse cx="120" cy="27" rx="9" ry="13" stroke="#E5C158" stroke-width="1.2"/>
                <line x1="104" y1="27" x2="136" y2="27" stroke="#E5C158" stroke-width="1.1"/>
                <line x1="120" y1="11" x2="120" y2="44" stroke="#E5C158" stroke-width="1.3"/>
                <rect x="114" y="13" width="12" height="3" rx="1" fill="#E5C158"/>
                <rect x="114" y="39" width="12" height="3" rx="1" fill="#E5C158"/>

                <!-- Nét vẽ Chùa Cầu Hội An góc trên phải -->
                <path d="M145 38 L192 38 M150 38 L150 30 L165 26 L180 30 L180 38 M156 38 A4 4 0 0 1 164 38 M168 38 A4 4 0 0 1 176 38" stroke="#E5C158" stroke-width="1.2" stroke-opacity="0.85"/>

                <!-- Lồng đèn tre đan phát sáng bên trái -->
                <ellipse cx="44" cy="92" rx="22" ry="25" fill="#D97706" fill-opacity="0.35" stroke="#F59E0B" stroke-width="2"/>
                <ellipse cx="44" cy="92" rx="11" ry="18" fill="#FEF3C7" fill-opacity="0.85"/>
                <path d="M26 80 L62 104 M26 104 L62 80 M32 70 L56 114 M32 114 L56 70" stroke="#92400E" stroke-width="1.2"/>
                <rect x="35" y="65" width="18" height="4" rx="1.5" fill="#B45309"/>
                <rect x="35" y="115" width="18" height="4" rx="1.5" fill="#B45309"/>
                <line x1="44" y1="119" x2="44" y2="133" stroke="#DC2626" stroke-width="2.2"/>

                <!-- Chữ CƠ SỞ SẢN XUẤT -->
                <text x="122" y="57" text-anchor="middle" fill="#FFFFFF" font-size="11" font-family="Inter, sans-serif" font-weight="600" letter-spacing="0.8">CƠ SỞ SẢN XUẤT</text>

                <!-- Chữ Lồng Đèn Hạnh Đào kiểu cọ thư pháp vàng -->
                <text x="122" y="88" text-anchor="middle" fill="#FDE68A" font-size="31" font-family="Playfair Display, serif" font-weight="700" font-style="italic">Lồng Đèn</text>
                <text x="122" y="118" text-anchor="middle" fill="#F5B041" font-size="31" font-family="Playfair Display, serif" font-weight="700" font-style="italic">Hạnh Đào</text>

                <!-- Ấn chương đỏ Hội An bên phải -->
                <rect x="190" y="88" width="24" height="30" rx="4" fill="#9E1B1B" stroke="#E5C158" stroke-width="1.1"/>
                <text x="202" y="101" text-anchor="middle" fill="#FFFFFF" font-size="8.5" font-family="Playfair Display, serif" font-style="italic">Hội</text>
                <text x="202" y="112" text-anchor="middle" fill="#FFFFFF" font-size="8.5" font-family="Playfair Display, serif" font-style="italic">An</text>

                <!-- Dải băng đỏ LỒNG ĐÈN TRE HỘI AN -->
                <rect x="64" y="125" width="116" height="14" rx="3" fill="#8B1515"/>
                <text x="122" y="135" text-anchor="middle" fill="#FDE68A" font-size="8.5" font-family="Inter, sans-serif" font-weight="700" letter-spacing="0.5">LỒNG ĐÈN TRE HỘI AN</text>

                <!-- Dòng chữ SẢN XUẤT TRỰC TIẾP - GIÁ TỐT TẠI XƯỞNG -->
                <text x="122" y="149" text-anchor="middle" fill="#F3F4F6" font-size="7" font-family="Inter, sans-serif" font-weight="600">SẢN XUẤT TRỰC TIẾP – GIÁ TỐT TẠI XƯỞNG</text>

                <!-- 5 vòng tròn icon cam kết -->
                <circle cx="72" cy="162" r="8" stroke="#E5C158" stroke-width="1.2" fill="#1C1917"/>
                <circle cx="97" cy="162" r="8" stroke="#E5C158" stroke-width="1.2" fill="#1C1917"/>
                <circle cx="122" cy="162" r="8" stroke="#E5C158" stroke-width="1.2" fill="#1C1917"/>
                <circle cx="147" cy="162" r="8" stroke="#E5C158" stroke-width="1.2" fill="#1C1917"/>
                <circle cx="172" cy="162" r="8" stroke="#E5C158" stroke-width="1.2" fill="#1C1917"/>

                <!-- Khung vàng Zalo 0796 693 304 -->
                <rect x="62" y="175" width="120" height="20" rx="10" fill="#E5C178"/>
                <circle cx="75" cy="185" r="7" fill="#7A1212"/>
                <text x="75" y="187.5" text-anchor="middle" fill="#FFFFFF" font-size="5.5" font-family="Inter, sans-serif" font-weight="700">Zalo</text>
                <text x="132" y="189" text-anchor="middle" fill="#5A0C0C" font-size="13" font-family="Inter, sans-serif" font-weight="800">0796 693 304</text>

                <!-- Khung đỏ 92 Nguyễn Du, Hội An -->
                <rect x="66" y="199" width="112" height="17" rx="8.5" fill="#4A1212" stroke="#E5C158" stroke-width="0.9"/>
                <text x="122" y="210" text-anchor="middle" fill="#FFFFFF" font-size="8.5" font-family="Inter, sans-serif" font-weight="700">92 Nguyễn Du, Hội An</text>

                <!-- Thắp sáng không gian Việt -->
                <text x="122" y="226" text-anchor="middle" fill="#FDE68A" font-size="8.5" font-family="Playfair Display, serif" font-style="italic">Thắp sáng không gian Việt ♡</text>
              </svg>
            </div>
          </div>
          <div>
            <span class="block font-serif font-bold text-lg md:text-2xl text-brand-red tracking-tight leading-none">
              LỒNG ĐÈN HẠNH ĐÀO
            </span>
            <span class="block text-[11px] md:text-xs text-stone-600 font-medium mt-1">
              Lồng đèn tre Hội An • Sản xuất trực tiếp tại xưởng
            </span>
          </div>
        </a>

        <!-- Thanh tìm kiếm sản phẩm (Chuẩn Flatsome Search Box) -->
        <div class="hidden md:flex flex-1 max-w-md mx-auto">
          <div class="relative w-full">
            <input 
              id="desktop-search" 
              type="text" 
              oninput="handleSearch(this.value)"
              placeholder="Tìm đèn lồng lụa, phi hoa 3D, đèn gỗ, đèn vẽ..." 
              class="w-full pl-4 pr-11 py-2.5 text-sm rounded-full border border-stone-300 focus:outline-none focus:border-brand-red bg-stone-50 focus:bg-white transition"
            >
            <button onclick="handleSearch(document.getElementById('desktop-search').value)" aria-label="Tìm kiếm" class="absolute right-1.5 top-1.5 bottom-1.5 px-3.5 bg-brand-red text-white rounded-full hover:bg-brand-darkRed transition">
              <i class="fa-solid fa-magnifying-glass text-xs"></i>
            </button>
          </div>
        </div>

        <!-- Cụm nút Hotline & Fanpage bên phải Header -->
        <div class="flex items-center gap-2.5 md:gap-3">
          <a href="tel:0796693304" class="hidden sm:flex items-center gap-2.5 px-3.5 py-2 rounded-xl bg-amber-50 border border-amber-200 hover:bg-amber-100 transition">
            <div class="w-8 h-8 rounded-full bg-brand-red text-white flex items-center justify-center shrink-0">
              <i class="fa-solid fa-phone text-xs"></i>
            </div>
            <div class="leading-tight">
              <span class="block text-[10px] uppercase tracking-wider text-stone-500 font-semibold">Hotline / Zalo Sỉ & Lẻ</span>
              <span class="block text-sm font-bold text-brand-red">0796.693.304</span>
            </div>
          </a>

          <a href="https://www.facebook.com/profile.php?id=61577469388669" target="_blank" rel="noopener noreferrer" class="px-3.5 py-2.5 rounded-xl bg-brand-red hover:bg-brand-darkRed text-white text-xs md:text-sm font-semibold flex items-center gap-2 shadow-sm transition">
            <i class="fa-brands fa-facebook-f"></i>
            <span class="hidden md:inline">Fanpage Hạnh Đào</span>
          </a>
        </div>

      </div>

      <!-- Thanh tìm kiếm trên Điện thoại -->
      <div class="mt-2.5 md:hidden">
        <div class="relative w-full">
          <input 
            id="mobile-search" 
            type="text" 
            oninput="handleSearch(this.value)"
            placeholder="Tìm mẫu đèn lồng Hội An..." 
            class="w-full pl-3.5 pr-10 py-2 text-sm rounded-lg border border-stone-300 bg-stone-50 focus:bg-white focus:outline-none focus:border-brand-red"
          >
          <button onclick="handleSearch(document.getElementById('mobile-search').value)" aria-label="Tìm kiếm" class="absolute right-2 top-1/2 -translate-y-1/2 text-brand-red p-1">
            <i class="fa-solid fa-magnifying-glass"></i>
          </button>
        </div>
      </div>
    </div>

    <!-- =========================================================
         3. THANH ĐIỀU HƯỚNG & MENU DANH MỤC TRÊN MÁY TÍNH (Tối ưu chuẩn Flatsome)
    ========================================================== -->
    <nav class="hidden lg:block bg-brand-red text-white border-t border-red-800">
      <div class="flatsome-container flex items-center justify-between">
        
        <!-- Nút Dropdown Danh Mục Sản Phẩm kiểu Flatsome Mega Menu -->
        <div class="relative group">
          <button class="bg-brand-darkRed px-5 py-3.5 font-bold text-xs uppercase tracking-wider flex items-center gap-3 min-w-[250px] justify-between border-x border-red-900/60">
            <span class="flex items-center gap-2.5">
              <i class="fa-solid fa-list-ul text-brand-gold"></i>
              <span>DANH MỤC SẢN PHẨM</span>
            </span>
            <i class="fa-solid fa-chevron-down text-[10px] text-amber-200 group-hover:rotate-180 transition-transform"></i>
          </button>

          <!-- Danh sách xổ xuống lấy từ denlongvn.com -->
          <div class="absolute left-0 top-full w-[270px] bg-white text-stone-800 shadow-xl rounded-b-xl border border-stone-200 py-2 hidden group-hover:block z-50">
            <a href="#san-pham" onclick="filterByCategory('all')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red font-medium border-b border-stone-100 transition">
              <span><i class="fa-solid fa-border-all w-5 text-brand-red"></i> Tất cả sản phẩm</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('den-long-hoi-an')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng Hội An (Lụa tơ tằm)</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('phi-hoa-3d')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng phi hoa 3D</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('vai-hoa-gam-truc')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng vải hoa & Gấm trúc</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('xo-voan-tho-cam')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng Xô Voan & Thổ cẩm</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('theu-tay-ve-hoa-tiet')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng thêu tay & Vẽ họa tiết</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('in-logo-su-kien')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng in Logo & Sự kiện</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('den-go-hoa-sen')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red border-b border-stone-100 transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn gỗ lục giác & Đèn hoa sen</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
            <a href="#san-pham" onclick="filterByCategory('den-long-nhat')" class="flex items-center justify-between px-4 py-2.5 text-sm hover:bg-red-50 hover:text-brand-red transition">
              <span><i class="fa-solid fa-circle-dot w-5 text-brand-red text-[10px]"></i> Đèn lồng kiểu Nhật</span>
              <i class="fa-solid fa-angle-right text-xs text-stone-400"></i>
            </a>
          </div>
        </div>

        <!-- Menu ngang trên máy tính -->
        <ul class="flex items-center gap-1 text-xs font-semibold uppercase tracking-wide">
          <li><a href="#" onclick="filterByCategory('all'); return false;" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Trang chủ</a></li>
          <li><a href="#san-pham" onclick="filterByCategory('den-long-hoi-an')" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Đèn lồng Hội An</a></li>
          <li><a href="#san-pham" onclick="filterByCategory('phi-hoa-3d')" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Phi hoa 3D</a></li>
          <li><a href="#san-pham" onclick="filterByCategory('vai-hoa-gam-truc')" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Vải hoa & Gấm</a></li>
          <li><a href="#san-pham" onclick="filterByCategory('xo-voan-tho-cam')" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Xô Voan & Thổ Cẩm</a></li>
          <li><a href="#san-pham" onclick="filterByCategory('theu-tay-ve-hoa-tiet')" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Đèn vẽ & Thêu tay</a></li>
          <li><a href="#san-pham" onclick="filterByCategory('den-go-hoa-sen')" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition">Đèn Gỗ & Hoa Sen</a></li>
          <li><a href="#ban-do-trang-chu" class="px-3.5 py-3.5 inline-block hover:bg-brand-darkRed transition text-amber-200"><i class="fa-solid fa-map-location-dot mr-1"></i>Bản đồ & Liên hệ</a></li>
        </ul>

      </div>
    </nav>
  </header>

  <!-- =========================================================
       MENU TRƯỢT MOBILE (Off-Canvas Menu chuẩn Flatsome)
  ========================================================== -->
  <div id="mobile-menu-backdrop" onclick="toggleMobileMenu()" class="fixed inset-0 bg-black/60 z-50 hidden transition-opacity"></div>
  <aside id="mobile-menu-drawer" class="fixed top-0 left-0 bottom-0 w-[290px] bg-white z-50 -translate-x-full transition-transform duration-300 flex flex-col shadow-2xl">
    <div class="p-4 bg-brand-red text-white flex items-center justify-between">
      <div>
        <div class="font-serif font-bold text-base">LỒNG ĐÈN HẠNH ĐÀO</div>
        <div class="text-xs text-amber-200">longdenhanhdao.com</div>
      </div>
      <button onclick="toggleMobileMenu()" aria-label="Đóng menu" class="w-8 h-8 rounded-full bg-white/10 flex items-center justify-center text-white">
        <i class="fa-solid fa-xmark"></i>
      </button>
    </div>
    <div class="p-3 bg-amber-50 border-b border-amber-200 text-xs text-stone-700">
      <div class="font-semibold text-brand-red">Danh mục sản phẩm (Chuẩn mẫu)</div>
    </div>
    <div class="flex-1 overflow-y-auto divide-y divide-stone-100 text-sm">
      <a href="#san-pham" onclick="filterByCategory('all'); toggleMobileMenu();" class="block px-4 py-3 font-semibold text-brand-red hover:bg-red-50">Tất cả sản phẩm</a>
      <a href="#san-pham" onclick="filterByCategory('den-long-hoi-an'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">1. Đèn lồng Hội An (Lụa tơ tằm)</a>
      <a href="#san-pham" onclick="filterByCategory('phi-hoa-3d'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">2. Đèn lồng phi hoa 3D</a>
      <a href="#san-pham" onclick="filterByCategory('vai-hoa-gam-truc'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">3. Đèn lồng vải hoa & Gấm trúc</a>
      <a href="#san-pham" onclick="filterByCategory('xo-voan-tho-cam'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">4. Đèn lồng Xô Voan & Thổ cẩm</a>
      <a href="#san-pham" onclick="filterByCategory('theu-tay-ve-hoa-tiet'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">5. Đèn lồng thêu tay & Vẽ họa tiết</a>
      <a href="#san-pham" onclick="filterByCategory('in-logo-su-kien'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">6. Đèn lồng in Logo & Sự kiện</a>
      <a href="#san-pham" onclick="filterByCategory('den-go-hoa-sen'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">7. Đèn gỗ lục giác & Đèn hoa sen</a>
      <a href="#san-pham" onclick="filterByCategory('den-long-nhat'); toggleMobileMenu();" class="block px-4 py-3 text-stone-700 hover:bg-red-50">8. Đèn lồng kiểu Nhật</a>
      <a href="#ban-do-trang-chu" onclick="toggleMobileMenu();" class="block px-4 py-3 font-semibold text-stone-800 hover:bg-red-50">
        <i class="fa-solid fa-location-dot text-brand-red mr-1.5"></i> Bản đồ: 92 Nguyễn Du, Hội An
      </a>
    </div>
    <div class="p-4 bg-stone-50 border-t border-stone-200 text-xs space-y-1.5">
      <div><strong>Địa chỉ:</strong> 92 Nguyễn Du, Hội An, Đà Nẵng</div>
      <div><strong>Hotline/Zalo:</strong> <a href="tel:0796693304" class="text-brand-red font-bold">0796.693.304</a></div>
    </div>
  </aside>

  <!-- =========================================================
       4. SLIDER 2 ẢNH BANNER TỰ TRƯỢT (Flatsome [ux_slider] + [ux_banner])
  ========================================================== -->
  <section class="py-3 md:py-5">
    <div class="flatsome-container">
      <div class="relative rounded-2xl overflow-hidden shadow-md bg-stone-900 h-[280px] sm:h-[370px] md:h-[440px]" id="hero-slider">
        
        <!-- SLIDE 1: Xưởng Sản Xuất Lồng Đèn Hạnh Đào (Kèm Logo ảnh tròn ở trên hiển thị nổi bật bên phải banner) -->
        <div class="hero-slide absolute inset-0 transition-opacity duration-700 opacity-100 z-10">
          <img 
            src="https://commons.wikimedia.org/wiki/Special:FilePath/Making_lanterns_in_Hoi_An_(31477021917).jpg?width=1400" 
            alt="Xưởng Sản Xuất Lồng Đèn Hạnh Đào Hội An" 
            class="w-full h-full object-cover object-center"
          >
          <div class="absolute inset-0 bg-gradient-to-r from-black/85 via-black/65 to-black/35 flex items-center">
            <div class="w-full px-6 sm:px-12 md:px-16 flex flex-col md:flex-row items-center justify-between gap-6">
              <div class="max-w-xl text-white space-y-2.5 md:space-y-4">
                <p class="text-amber-300 text-xs md:text-sm font-semibold uppercase tracking-widest">
                  Cơ Sở Sản Xuất Lồng Đèn Tre Hội An • longdenhanhdao.com
                </p>
                <h1 class="font-serif text-2xl sm:text-4xl md:text-5xl font-bold leading-tight text-white">
                  Lồng Đèn Hạnh Đào <br><span class="text-amber-300">Sản Xuất Trực Tiếp – Giá Xưởng</span>
                </h1>
                <p class="text-xs sm:text-sm md:text-base text-stone-200 leading-relaxed">
                  Chất liệu tre tự nhiên • Thủ công tỉ mỉ • Bền đẹp thân thiện • Sỉ & lẻ toàn quốc. Địa chỉ: 92 Nguyễn Du, Hội An, Đà Nẵng.
                </p>
                <div class="pt-1 flex flex-wrap items-center gap-3">
                  <a href="#san-pham" class="px-5 py-2.5 rounded-full bg-brand-red hover:bg-brand-darkRed text-white font-semibold text-xs md:text-sm border border-amber-300/40 transition shadow">
                    Xem mẫu đèn lồng thực tế
                  </a>
                  <a href="tel:0796693304" class="px-5 py-2.5 rounded-full bg-amber-400 hover:bg-amber-300 text-stone-900 font-bold text-xs md:text-sm transition shadow">
                    <i class="fa-solid fa-phone mr-1.5"></i> Zalo: 0796.693.304
                  </a>
                </div>
              </div>

              <!-- Hiển thị Logo tròn Lồng Đèn Hạnh Đào trên Banner máy tính -->
              <div class="hidden md:flex shrink-0">
                <div class="w-56 h-56 lg:w-64 lg:h-64 rounded-full border-2 border-[#E5C158] shadow-2xl overflow-hidden bg-[#0b0908] relative">
                  <img 
                    src="image_c19582.jpg" 
                    alt="Logo Lồng Đèn Hạnh Đào Hội An" 
                    class="w-full h-full object-cover"
                    onerror="this.style.display='none'; document.getElementById('banner-logo-fallback').style.display='block';"
                  >
                  <div id="banner-logo-fallback" style="display:none;" class="w-full h-full relative bg-[#0b0908]">
                    <img 
                      src="https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An,_Vietnam_(25708206924).jpg?width=500" 
                      alt="" 
                      class="absolute inset-0 w-full h-full object-cover opacity-35"
                    >
                    <div class="absolute inset-0 bg-gradient-to-b from-black/80 via-black/65 to-black/90"></div>
                    <svg class="relative z-10 w-full h-full" viewBox="0 0 240 240" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <circle cx="120" cy="120" r="116" stroke="#E5C158" stroke-width="3.5"/>
                      <ellipse cx="120" cy="27" rx="16" ry="13" stroke="#E5C158" stroke-width="1.6"/>
                      <ellipse cx="120" cy="27" rx="9" ry="13" stroke="#E5C158" stroke-width="1.2"/>
                      <line x1="104" y1="27" x2="136" y2="27" stroke="#E5C158" stroke-width="1.1"/>
                      <path d="M145 38 L192 38 M150 38 L150 30 L165 26 L180 30 L180 38" stroke="#E5C158" stroke-width="1.2" stroke-opacity="0.85"/>
                      <ellipse cx="44" cy="92" rx="22" ry="25" fill="#D97706" fill-opacity="0.35" stroke="#F59E0B" stroke-width="2"/>
                      <ellipse cx="44" cy="92" rx="11" ry="18" fill="#FEF3C7" fill-opacity="0.85"/>
                      <path d="M26 80 L62 104 M26 104 L62 80 M32 70 L56 114 M32 114 L56 70" stroke="#92400E" stroke-width="1.2"/>
                      <text x="122" y="57" text-anchor="middle" fill="#FFFFFF" font-size="11" font-family="Inter, sans-serif" font-weight="600" letter-spacing="0.8">CƠ SỞ SẢN XUẤT</text>
                      <text x="122" y="88" text-anchor="middle" fill="#FDE68A" font-size="31" font-family="Playfair Display, serif" font-weight="700" font-style="italic">Lồng Đèn</text>
                      <text x="122" y="118" text-anchor="middle" fill="#F5B041" font-size="31" font-family="Playfair Display, serif" font-weight="700" font-style="italic">Hạnh Đào</text>
                      <rect x="190" y="88" width="24" height="30" rx="4" fill="#9E1B1B" stroke="#E5C158" stroke-width="1.1"/>
                      <text x="202" y="101" text-anchor="middle" fill="#FFFFFF" font-size="8.5" font-family="Playfair Display, serif" font-style="italic">Hội</text>
                      <text x="202" y="112" text-anchor="middle" fill="#FFFFFF" font-size="8.5" font-family="Playfair Display, serif" font-style="italic">An</text>
                      <rect x="64" y="125" width="116" height="14" rx="3" fill="#8B1515"/>
                      <text x="122" y="135" text-anchor="middle" fill="#FDE68A" font-size="8.5" font-family="Inter, sans-serif" font-weight="700" letter-spacing="0.5">LỒNG ĐÈN TRE HỘI AN</text>
                      <text x="122" y="149" text-anchor="middle" fill="#F3F4F6" font-size="7" font-family="Inter, sans-serif" font-weight="600">SẢN XUẤT TRỰC TIẾP – GIÁ TỐT TẠI XƯỞNG</text>
                      <circle cx="72" cy="162" r="7.5" stroke="#E5C158" stroke-width="1.2" fill="#1C1917"/>
                      <circle cx="97" cy="162" r="7.5" stroke="#E5C158" stroke-width="1.2" fill="#1C1917"/>
                      <circle cx="122" cy="162" r="7.5" stroke="#E5C158" stroke-width="1.2" fill="#1C1917"/>
                      <circle cx="147" cy="162" r="7.5" stroke="#E5C158" stroke-width="1.2" fill="#1C1917"/>
                      <circle cx="172" cy="162" r="7.5" stroke="#E5C158" stroke-width="1.2" fill="#1C1917"/>
                      <rect x="62" y="175" width="120" height="20" rx="10" fill="#E5C178"/>
                      <circle cx="75" cy="185" r="7" fill="#7A1212"/>
                      <text x="75" y="187.5" text-anchor="middle" fill="#FFFFFF" font-size="5.5" font-family="Inter, sans-serif" font-weight="700">Zalo</text>
                      <text x="132" y="189" text-anchor="middle" fill="#5A0C0C" font-size="13" font-family="Inter, sans-serif" font-weight="800">0796 693 304</text>
                      <rect x="66" y="199" width="112" height="17" rx="8.5" fill="#4A1212" stroke="#E5C158" stroke-width="0.9"/>
                      <text x="122" y="210" text-anchor="middle" fill="#FFFFFF" font-size="8.5" font-family="Inter, sans-serif" font-weight="700">92 Nguyễn Du, Hội An</text>
                      <text x="122" y="226" text-anchor="middle" fill="#FDE68A" font-size="8.5" font-family="Playfair Display, serif" font-style="italic">Thắp sáng không gian Việt ♡</text>
                    </svg>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- SLIDE 2: Không gian Đèn Lồng Hội An thực tế đủ kiểu dáng và màu sắc -->
        <div class="hero-slide absolute inset-0 transition-opacity duration-700 opacity-0 z-0">
          <img 
            src="https://commons.wikimedia.org/wiki/Special:FilePath/Hoi_An_Laternen_und_Lampions_(39543426861).jpg?width=1400" 
            alt="Đèn lồng lụa tơ tằm, đèn lồng tre và phi hoa 3D Hội An" 
            class="w-full h-full object-cover object-center"
          >
          <div class="absolute inset-0 bg-gradient-to-r from-red-950/85 via-stone-900/60 to-transparent flex items-center">
            <div class="px-6 sm:px-12 md:px-16 max-w-2xl text-white space-y-2.5 md:space-y-4">
              <p class="text-amber-300 text-xs md:text-sm font-semibold uppercase tracking-widest">
                92 Nguyễn Du, Hội An, Đà Nẵng
              </p>
              <h2 class="font-serif text-2xl sm:text-4xl md:text-5xl font-bold leading-tight text-white">
                Lồng Đèn Tre Tự Nhiên <br><span class="text-amber-300">& Đèn Lồng Lụa Hội An</span>
              </h2>
              <p class="text-xs sm:text-sm md:text-base text-stone-200 leading-relaxed">
                Đầy đủ mẫu đèn lồng tròn, tỏi, na, dù, kim cương, bánh ú, đèn tre đan, đèn gỗ lục giác & hoa sen. Nhận đặt sỉ & lẻ giao toàn quốc.
              </p>
              <div class="pt-1 flex flex-wrap items-center gap-3">
                <a href="https://zalo.me/0796693304" target="_blank" rel="noopener noreferrer" class="px-5 py-2.5 rounded-full bg-amber-400 hover:bg-amber-300 text-stone-900 font-bold text-xs md:text-sm transition shadow">
                  Nhận báo giá sỉ qua Zalo
                </a>
                <a href="#ban-do-trang-chu" class="px-5 py-2.5 rounded-full bg-white/15 hover:bg-white/25 backdrop-blur text-white font-semibold text-xs md:text-sm border border-white/30 transition">
                  Chỉ đường đến xưởng
                </a>
              </div>
            </div>
          </div>
        </div>

        <!-- Nút điều hướng Trái / Phải của Banner -->
        <button onclick="changeSlide(-1)" aria-label="Banner trước" class="absolute left-3 top-1/2 -translate-y-1/2 z-20 w-9 h-9 md:w-10 md:h-10 rounded-full bg-black/40 hover:bg-brand-red text-white flex items-center justify-center transition">
          <i class="fa-solid fa-chevron-left text-sm"></i>
        </button>
        <button onclick="changeSlide(1)" aria-label="Banner tiếp" class="absolute right-3 top-1/2 -translate-y-1/2 z-20 w-9 h-9 md:w-10 md:h-10 rounded-full bg-black/40 hover:bg-brand-red text-white flex items-center justify-center transition">
          <i class="fa-solid fa-chevron-right text-sm"></i>
        </button>

        <!-- Dấu chấm chuyển Slide -->
        <div class="absolute bottom-3.5 left-1/2 -translate-x-1/2 z-20 flex items-center gap-2">
          <button onclick="goToSlide(0)" id="dot-0" aria-label="Banner 1" class="w-7 h-2 rounded-full bg-amber-400 transition-all"></button>
          <button onclick="goToSlide(1)" id="dot-1" aria-label="Banner 2" class="w-2.5 h-2 rounded-full bg-white/60 transition-all"></button>
        </div>

      </div>
    </div>
  </section>

  <!-- =========================================================
       5. DANH MỤC SẢN PHẨM (Tối ưu hiển thị đẹp trên cả Máy tính & Điện thoại)
          Lấy từ danh mục web mẫu denlongvn.com
  ========================================================== -->
  <section class="py-5 md:py-8">
    <div class="flatsome-container">
      
      <div class="section-title-container">
        <div class="section-title-line"></div>
        <h2 class="section-title-text text-base md:text-xl font-serif">DANH MỤC ĐÈN LỒNG HỘI AN</h2>
        <div class="section-title-line"></div>
      </div>

      <!-- Bố cục: 4 cột gọn đẹp trên điện thoại (2 hàng x 4) và 8 cột sang trọng trên máy tính -->
      <div class="grid grid-cols-4 lg:grid-cols-8 gap-2.5 sm:gap-4" id="category-visual-grid">
        <!-- Render động từ danh sách danh mục chuẩn denlongvn.com -->
      </div>

      <!-- Thanh nút lọc nhanh hỗ trợ UX Builder -->
      <div class="mt-5 flex items-center justify-start md:justify-center gap-2 overflow-x-auto no-scrollbar pb-1" id="category-pills">
        <!-- Render động các pill danh mục -->
      </div>

    </div>
  </section>

  <!-- =========================================================
       6. DANH SÁCH SẢN PHẨM THEO DANH MỤC (Chuẩn Flatsome Section, 2 cột trên Điện thoại, 4 cột trên Máy tính)
          LƯU Ý: KHÔNG ĐỂ CÁC NHÃN DÁN (SALE/HOT/NEW) Ở TRANG CHỦ
  ========================================================== -->
  <main id="san-pham" class="py-4 md:py-6 space-y-10">
    <div class="flatsome-container" id="product-sections-wrapper">
      <!-- Render các Section sản phẩm theo đúng cấu trúc Row/Col của Flatsome -->
    </div>
  </main>

  <!-- =========================================================
       7. ĐẶC ĐIỂM XƯỞNG LỒNG ĐÈN HẠNH ĐÀO (Flatsome 4-Col Featured Box)
  ========================================================== -->
  <section class="py-8 bg-white border-y border-stone-200">
    <div class="flatsome-container">
      <div class="grid grid-cols-2 lg:grid-cols-4 gap-4 md:gap-6">
        <div class="p-4 rounded-xl bg-brand-bg border border-stone-200/80 text-center space-y-1.5">
          <div class="w-11 h-11 mx-auto rounded-full bg-red-50 text-brand-red flex items-center justify-center text-lg">
            <i class="fa-solid fa-hammer"></i>
          </div>
          <h3 class="font-bold text-sm md:text-base text-stone-800">Giá Gốc Tại Xưởng</h3>
          <p class="text-xs text-stone-600">Sản xuất trực tiếp tại 92 Nguyễn Du, Hội An không qua trung gian.</p>
        </div>

        <div class="p-4 rounded-xl bg-brand-bg border border-stone-200/80 text-center space-y-1.5">
          <div class="w-11 h-11 mx-auto rounded-full bg-red-50 text-brand-red flex items-center justify-center text-lg">
            <i class="fa-solid fa-palette"></i>
          </div>
          <h3 class="font-bold text-sm md:text-base text-stone-800">Nhận Làm Theo Yêu Cầu</h3>
          <p class="text-xs text-stone-600">Đặt kích thước riêng, vẽ tay, thêu hoa văn và in logo thương hiệu.</p>
        </div>

        <div class="p-4 rounded-xl bg-brand-bg border border-stone-200/80 text-center space-y-1.5">
          <div class="w-11 h-11 mx-auto rounded-full bg-red-50 text-brand-red flex items-center justify-center text-lg">
            <i class="fa-solid fa-medal"></i>
          </div>
          <h3 class="font-bold text-sm md:text-base text-stone-800">Tre Xử Lý & Lụa Cao Cấp</h3>
          <p class="text-xs text-stone-600">Khung tre già xử lý chống mối mọt, bọc lụa tơ tằm, gấm, phi hoa 3D bền màu.</p>
        </div>

        <div class="p-4 rounded-xl bg-brand-bg border border-stone-200/80 text-center space-y-1.5">
          <div class="w-11 h-11 mx-auto rounded-full bg-red-50 text-brand-red flex items-center justify-center text-lg">
            <i class="fa-solid fa-truck-fast"></i>
          </div>
          <h3 class="font-bold text-sm md:text-base text-stone-800">Giao Hàng Toàn Quốc</h3>
          <p class="text-xs text-stone-600">Đóng gói xếp gọn an toàn, vận chuyển nhanh chóng khắp 63 tỉnh thành.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- =========================================================
       8. BẢN ĐỒ GOOGLE MAPS NGOÀI TRANG CHỦ & THÔNG TIN LIÊN HỆ
          Địa chỉ: 92 Nguyễn Du, Hội An, Đà Nẵng | SĐT: 0796.693.304
  ========================================================== -->
  <section id="ban-do-trang-chu" class="py-8 md:py-12">
    <div class="flatsome-container">
      
      <div class="section-title-container">
        <div class="section-title-line"></div>
        <h2 class="section-title-text text-base md:text-xl font-serif">BẢN ĐỒ ĐẾN XƯỞNG LỒNG ĐÈN HẠNH ĐÀO</h2>
        <div class="section-title-line"></div>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 bg-white p-4 sm:p-6 rounded-2xl shadow-sm border border-stone-200">
        
        <!-- Cột trái: Thông tin xưởng & Đặt hàng nhanh (5 cột) -->
        <div class="lg:col-span-5 flex flex-col justify-between space-y-5">
          <div class="space-y-4">
            <div>
              <h3 class="font-serif font-bold text-xl text-brand-red">Cơ Sở Sản Xuất Lồng Đèn Hạnh Đào</h3>
              <p class="text-xs text-stone-500 mt-0.5">Website chính thức: <strong>longdenhanhdao.com</strong></p>
            </div>

            <div class="space-y-3 text-sm text-stone-700">
              <div class="flex items-start gap-3">
                <div class="w-8 h-8 rounded-lg bg-red-50 text-brand-red flex items-center justify-center shrink-0 mt-0.5">
                  <i class="fa-solid fa-location-dot"></i>
                </div>
                <div>
                  <span class="font-semibold text-stone-900 block">Địa chỉ xưởng & cửa hàng:</span>
                  <span>92 Nguyễn Du, Hội An, Đà Nẵng</span>
                </div>
              </div>

              <div class="flex items-start gap-3">
                <div class="w-8 h-8 rounded-lg bg-red-50 text-brand-red flex items-center justify-center shrink-0 mt-0.5">
                  <i class="fa-solid fa-phone-volume"></i>
                </div>
                <div>
                  <span class="font-semibold text-stone-900 block">Điện thoại / Zalo tư vấn sỉ & lẻ:</span>
                  <a href="tel:0796693304" class="text-brand-red font-bold text-base hover:underline">0796.693.304</a>
                </div>
              </div>

              <div class="flex items-start gap-3">
                <div class="w-8 h-8 rounded-lg bg-red-50 text-brand-red flex items-center justify-center shrink-0 mt-0.5">
                  <i class="fa-brands fa-facebook"></i>
                </div>
                <div>
                  <span class="font-semibold text-stone-900 block">Fanpage Facebook:</span>
                  <a href="https://www.facebook.com/profile.php?id=61577469388669" target="_blank" rel="noopener noreferrer" class="text-blue-600 hover:underline break-all">
                    facebook.com/profile.php?id=61577469388669
                  </a>
                </div>
              </div>
            </div>
          </div>

          <!-- Form gửi yêu cầu báo giá sỉ/lẻ nhanh -->
          <form onsubmit="submitQuickQuote(event)" class="p-4 rounded-xl bg-stone-50 border border-stone-200 space-y-3">
            <div class="font-bold text-sm text-stone-800">Nhận báo giá sỉ / Đặt đèn theo yêu cầu</div>
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-2.5">
              <input type="text" id="quote-name" required placeholder="Tên của bạn *" class="w-full px-3 py-2 text-xs rounded-lg border border-stone-300 bg-white focus:outline-none focus:border-brand-red">
              <input type="tel" id="quote-phone" required placeholder="Số điện thoại / Zalo *" class="w-full px-3 py-2 text-xs rounded-lg border border-stone-300 bg-white focus:outline-none focus:border-brand-red">
            </div>
            <input type="text" id="quote-note" placeholder="Loại đèn & số lượng cần báo giá (VD: 50 đèn lụa 30cm)..." class="w-full px-3 py-2 text-xs rounded-lg border border-stone-300 bg-white focus:outline-none focus:border-brand-red">
            <button type="submit" class="w-full py-2.5 rounded-lg bg-brand-red hover:bg-brand-darkRed text-white font-semibold text-xs uppercase tracking-wider transition">
              Gửi yêu cầu báo giá
            </button>
            <p id="quote-success" class="hidden text-xs text-emerald-700 font-medium text-center pt-1"></p>
          </form>
        </div>

        <!-- Cột phải: Bản đồ Google Maps hiển thị trực tiếp ngoài trang chủ (7 cột) -->
        <div class="lg:col-span-7 flex flex-col space-y-2.5">
          <div class="relative w-full h-[320px] sm:h-[380px] rounded-xl overflow-hidden border border-stone-300 bg-stone-100 shadow-inner">
            <iframe 
              title="Bản đồ Google Map Lồng Đèn Hạnh Đào 92 Nguyễn Du, Hội An"
              src="https://maps.google.com/maps?q=92%20Nguy%E1%BB%85n%20Du,%20H%E1%BB%99i%20An&t=&z=16&ie=UTF8&iwloc=&output=embed" 
              class="w-full h-full border-0" 
              allowfullscreen="" 
              loading="lazy" 
              referrerpolicy="no-referrer-when-downgrade">
            </iframe>
          </div>
          <div class="flex flex-wrap items-center justify-between gap-2 text-xs text-stone-600 px-1">
            <span><i class="fa-solid fa-map-pin text-brand-red mr-1"></i> <strong>Vị trí trên bản đồ:</strong> 92 Nguyễn Du, Hội An, Đà Nẵng</span>
            <a 
              href="https://www.google.com/maps/search/?api=1&query=92+Nguyen+Du+Hoi+An" 
              target="_blank" 
              rel="noopener noreferrer" 
              class="inline-flex items-center gap-1.5 font-semibold text-brand-red hover:underline"
            >
              <span>Mở trên ứng dụng Google Maps</span>
              <i class="fa-solid fa-arrow-up-right-from-square text-[10px]"></i>
            </a>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- =========================================================
       9. FOOTER CHUẨN FLATSOME (4 Cột đơn giản, dễ chỉnh sửa trên UX Builder)
  ========================================================== -->
  <footer class="bg-stone-900 text-stone-300 pt-10 pb-6 border-t-4 border-brand-red">
    <div class="flatsome-container">
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 pb-8 border-b border-stone-800 text-sm">
        
        <!-- Cột 1 -->
        <div class="space-y-3">
          <div class="font-serif font-bold text-lg text-amber-400">LỒNG ĐÈN HẠNH ĐÀO</div>
          <p class="text-xs text-stone-400 leading-relaxed">
            Xưởng chuyên sản xuất và cung cấp sỉ & lẻ các loại đèn lồng Hội An truyền thống, đèn lồng lụa tơ tằm, phi hoa 3D, gấm trúc, đèn gỗ lục giác, đèn hoa sen trang trí phòng, quán cafe, nhà hàng và sự kiện.
          </p>
          <div class="text-xs text-amber-300 font-medium">Website: longdenhanhdao.com</div>
        </div>

        <!-- Cột 2 -->
        <div class="space-y-3">
          <div class="font-bold text-white uppercase tracking-wider text-xs">Danh Mục Sản Phẩm</div>
          <ul class="space-y-2 text-xs text-stone-400">
            <li><a href="#san-pham" onclick="filterByCategory('den-long-hoi-an')" class="hover:text-amber-300 transition">• Đèn lồng Hội An lụa tơ tằm</a></li>
            <li><a href="#san-pham" onclick="filterByCategory('phi-hoa-3d')" class="hover:text-amber-300 transition">• Đèn lồng phi hoa 3D</a></li>
            <li><a href="#san-pham" onclick="filterByCategory('vai-hoa-gam-truc')" class="hover:text-amber-300 transition">• Đèn lồng vải hoa & Gấm trúc</a></li>
            <li><a href="#san-pham" onclick="filterByCategory('xo-voan-tho-cam')" class="hover:text-amber-300 transition">• Đèn lồng Xô Voan & Thổ cẩm</a></li>
            <li><a href="#san-pham" onclick="filterByCategory('theu-tay-ve-hoa-tiet')" class="hover:text-amber-300 transition">• Đèn lồng thêu tay & Vẽ họa tiết</a></li>
            <li><a href="#san-pham" onclick="filterByCategory('den-go-hoa-sen')" class="hover:text-amber-300 transition">• Đèn gỗ & Đèn hoa sen</a></li>
          </ul>
        </div>

        <!-- Cột 3 -->
        <div class="space-y-3">
          <div class="font-bold text-white uppercase tracking-wider text-xs">Hỗ Trợ Khách Hàng</div>
          <ul class="space-y-2 text-xs text-stone-400">
            <li>• Tư vấn chọn kích thước đèn (20cm - 80cm)</li>
            <li>• Chính sách chiết khấu đơn hàng sỉ & dự án</li>
            <li>• Hướng dẫn bung mở và bảo quản đèn lồng</li>
            <li>• Ship COD toàn quốc & gửi xe đi các tỉnh</li>
          </ul>
        </div>

        <!-- Cột 4 -->
        <div class="space-y-3">
          <div class="font-bold text-white uppercase tracking-wider text-xs">Thông Tin Liên Hệ</div>
          <ul class="space-y-2 text-xs text-stone-300">
            <li><i class="fa-solid fa-location-dot text-amber-400 w-4"></i> 92 Nguyễn Du, Hội An, Đà Nẵng</li>
            <li><i class="fa-solid fa-phone text-amber-400 w-4"></i> Hotline/Zalo: <a href="tel:0796693304" class="font-bold text-amber-300">0796.693.304</a></li>
            <li><i class="fa-solid fa-globe text-amber-400 w-4"></i> Website: longdenhanhdao.com</li>
            <li>
              <a href="https://www.facebook.com/profile.php?id=61577469388669" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-1.5 mt-1 px-3 py-1.5 rounded bg-blue-600 hover:bg-blue-500 text-white text-xs font-medium transition">
                <i class="fa-brands fa-facebook-f"></i> Kết nối Fanpage Hạnh Đào
              </a>
            </li>
          </ul>
        </div>

      </div>

      <div class="pt-5 flex flex-col sm:flex-row items-center justify-between gap-2 text-xs text-stone-500">
        <div>© Bản quyền thuộc về <strong>Lồng Đèn Hạnh Đào (longdenhanhdao.com)</strong> – 92 Nguyễn Du, Hội An, Đà Nẵng.</div>
        <div>Thiết kế giao diện chuẩn Flatsome</div>
      </div>
    </div>
  </footer>

  <!-- =========================================================
       10. CÁC NÚT LIÊN HỆ NỔI BẬT (ZALO, FACEBOOK, HOTLINE)
  ========================================================== -->
  <div class="fixed bottom-4 left-4 z-50 flex flex-col gap-3">
    
    <!-- Nút Facebook Fanpage nổi bật -->
    <a 
      href="https://www.facebook.com/profile.php?id=61577469388669" 
      target="_blank" 
      rel="noopener noreferrer"
      title="Nhắn tin Facebook Lồng Đèn Hạnh Đào"
      class="flex items-center gap-2.5 bg-[#1877F2] hover:bg-[#1464cc] text-white px-3.5 py-2.5 rounded-full shadow-lg transition transform hover:-translate-y-0.5"
    >
      <span class="w-7 h-7 rounded-full bg-white text-[#1877F2] flex items-center justify-center font-bold text-base shrink-0">
        <i class="fa-brands fa-facebook-f"></i>
      </span>
      <span class="text-xs font-bold pr-1">Facebook</span>
    </a>

    <!-- Nút Chat Zalo nổi bật -->
    <a 
      href="https://zalo.me/0796693304" 
      target="_blank" 
      rel="noopener noreferrer"
      title="Chat Zalo 0796.693.304"
      class="flex items-center gap-2.5 bg-[#0068FF] hover:bg-[#0056d6] text-white px-3.5 py-2.5 rounded-full shadow-lg animate-pulse-blue transition transform hover:-translate-y-0.5"
    >
      <span class="w-7 h-7 rounded-full bg-white text-[#0068FF] flex items-center justify-center font-extrabold text-[11px] tracking-tighter shrink-0">
        Zalo
      </span>
      <span class="text-xs font-bold pr-1">Zalo: 0796.693.304</span>
    </a>

    <!-- Nút Gọi Hotline nổi bật -->
    <a 
      href="tel:0796693304" 
      title="Gọi ngay 0796.693.304"
      class="flex items-center gap-2.5 bg-red-600 hover:bg-red-700 text-white px-3.5 py-2.5 rounded-full shadow-lg animate-pulse-red transition transform hover:-translate-y-0.5"
    >
      <span class="w-7 h-7 rounded-full bg-white text-red-600 flex items-center justify-center text-sm shrink-0">
        <i class="fa-solid fa-phone-volume"></i>
      </span>
      <span class="text-xs font-bold pr-1">0796.693.304</span>
    </a>

  </div>

  <!-- =========================================================
       MODAL CHI TIẾT SẢN PHẨM & ĐẶT HÀNG NHANH
  ========================================================== -->
  <div id="product-modal" class="fixed inset-0 bg-black/60 z-50 hidden items-center justify-center p-4">
    <div class="bg-white rounded-2xl max-w-lg w-full overflow-hidden shadow-2xl border border-stone-200 relative">
      <button onclick="closeProductModal()" aria-label="Đóng" class="absolute top-3 right-3 w-8 h-8 rounded-full bg-stone-100 hover:bg-stone-200 text-stone-700 flex items-center justify-center z-10">
        <i class="fa-solid fa-xmark"></i>
      </button>
      <div class="grid grid-cols-1 sm:grid-cols-12">
        <div class="sm:col-span-5 bg-stone-100">
          <img id="modal-img" src="" alt="" class="w-full h-56 sm:h-full object-cover">
        </div>
        <div class="sm:col-span-7 p-5 space-y-3">
          <div id="modal-cat" class="text-xs text-stone-500 font-medium"></div>
          <h3 id="modal-title" class="font-serif font-bold text-lg text-stone-900"></h3>
          <div id="modal-price" class="text-base font-bold text-brand-red"></div>
          <p id="modal-desc" class="text-xs text-stone-600 leading-relaxed"></p>
          <div class="text-xs text-stone-700 space-y-1 pt-1 border-t border-stone-100">
            <div><strong>Kích thước phổ biến:</strong> 20cm, 30cm, 35cm, 40cm, 45cm, 60cm</div>
            <div><strong>Kiểu dáng:</strong> Tròn, Tỏi, Na, Dù, Kim cương, Bánh ú, Trụ</div>
          </div>
          <div class="pt-2 flex flex-col gap-2">
            <a href="https://zalo.me/0796693304" target="_blank" rel="noopener noreferrer" class="w-full py-2.5 rounded-lg bg-[#0068FF] hover:bg-blue-700 text-white font-semibold text-xs text-center transition">
              Nhắn Zalo đặt mẫu này (0796.693.304)
            </a>
            <a href="tel:0796693304" class="w-full py-2.5 rounded-lg bg-brand-red hover:bg-brand-darkRed text-white font-semibold text-xs text-center transition">
              Gọi trực tiếp: 0796.693.304
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- =========================================================
       JAVASCRIPT: DỮ LIỆU DANH MỤC & SẢN PHẨM + SLIDER TỰ TRƯỢT
  ========================================================== -->
  <script>
    // 1. Danh mục sản phẩm mở rộng chuẩn denlongvn.com & Fanpage Lồng Đèn Hạnh Đào
    const categories = [
      {
        id: 'den-long-hoi-an',
        name: 'Đèn lồng Hội An',
        shortName: 'Đèn Hội An',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Hoi_An_lantern_lampion_(38834258624).jpg?width=400'
      },
      {
        id: 'phi-hoa-3d',
        name: 'Đèn lồng phi hoa 3D',
        shortName: 'Phi hoa 3D',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An_1.jpg?width=400'
      },
      {
        id: 'vai-hoa-gam-truc',
        name: 'Vải hoa & Gấm trúc',
        shortName: 'Vải hoa & Gấm',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lantern_Shop_in_Hoi_An_1.jpg?width=400'
      },
      {
        id: 'xo-voan-tho-cam',
        name: 'Xô Voan & Thổ cẩm',
        shortName: 'Xô Voan & Thổ cẩm',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An_5.jpg?width=400'
      },
      {
        id: 'theu-tay-ve-hoa-tiet',
        name: 'Thêu tay & Vẽ họa tiết',
        shortName: 'Thêu & Vẽ tay',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Hoi_An_lantern_lights_(39513532072).jpg?width=400'
      },
      {
        id: 'in-logo-su-kien',
        name: 'Đèn lồng in Logo',
        shortName: 'In Logo & Sự kiện',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Chinese_New_Year_(Tet_Festival)_Lampion.jpg?width=400'
      },
      {
        id: 'den-go-hoa-sen',
        name: 'Đèn tre, Gỗ & Hoa sen',
        shortName: 'Đèn tre, Gỗ & Sen',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Making_lanterns_in_Hoi_An_(31477021917).jpg?width=400'
      },
      {
        id: 'den-long-nhat',
        name: 'Đèn lồng kiểu Nhật',
        shortName: 'Đèn kiểu Nhật',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Paper_lantern.jpg?width=400'
      }
    ];

    // 2. Danh sách sản phẩm thực tế mở rộng hiển thị nhiều trên trang chủ (Không có nhãn dán)
    const products = [
      // Nhóm 1: Đèn lồng Hội An
      {
        id: 101,
        catId: 'den-long-hoi-an',
        catName: 'Đèn lồng Hội An',
        name: 'Đèn lồng Hội An lụa tơ tằm kiểu tròn truyền thống đủ màu',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An,_Vietnam_(25708206924).jpg?width=600',
        desc: 'Đèn lồng Hội An khung tre già xử lý chống mối mọt, bọc vải lụa tơ tằm trơn đủ màu sắc (đỏ, vàng, cam, xanh, tím, hồng) sản xuất trực tiếp tại xưởng Hạnh Đào.'
      },
      {
        id: 102,
        catId: 'den-long-hoi-an',
        catName: 'Đèn lồng Hội An',
        name: 'Đèn lồng Hội An kiểu củ tỏi lụa Hà Đông cao cấp',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Hoi_An_lantern_lampion_(38834258624).jpg?width=600',
        desc: 'Mẫu đèn lồng kiểu củ tỏi đặc trưng của phố cổ Hội An, thích hợp phối treo nhà hàng, quán cà phê, hiên nhà và không gian lễ hội.'
      },
      {
        id: 103,
        catId: 'den-long-hoi-an',
        catName: 'Đèn lồng Hội An',
        name: 'Đèn lồng Hội An kiểu quả Na & kiểu Trám thon dài',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An_(26652147368).jpg?width=600',
        desc: 'Thiết kế dáng quả Na và dáng Trám thanh thoát, dễ bung mở, tạo điểm nhấn ánh sáng ấm áp cho sân vườn, resort và khách sạn.'
      },
      {
        id: 104,
        catId: 'den-long-hoi-an',
        catName: 'Đèn lồng Hội An',
        name: 'Combo rèm đèn lồng Hội An đủ cỡ trang trí không gian',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Hoi_An_Laternen_und_Lampions_(39543426861).jpg?width=600',
        desc: 'Bộ phối các kiểu đèn tròn, tỏi, na, dù, kim cương kích thước từ 20cm đến 60cm dùng treo rèm, trần nhà hàng và phố đi bộ.'
      },

      // Nhóm 2: Đèn lồng phi hoa 3D
      {
        id: 201,
        catId: 'phi-hoa-3d',
        catName: 'Đèn lồng phi hoa 3D',
        name: 'Bộ đèn lồng vải phi hoa 3D Hội An phối đủ màu sắc',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An_1.jpg?width=600',
        desc: 'Chất liệu vải phi hoa 3D bóng đẹp, họa tiết hoa nổi bật sắc nét cả ban ngày lẫn khi thắp sáng vào ban đêm.'
      },
      {
        id: 202,
        catId: 'phi-hoa-3d',
        catName: 'Đèn lồng phi hoa 3D',
        name: 'Combo đèn lồng phi hoa 35cm treo tường & hiên nhà',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An_2.jpg?width=600',
        desc: 'Bộ đèn lồng phi hoa 3D kích thước 35cm chuyên dùng trang trí mặt tiền quán ăn, quán cafe, homestay và cổng chào.'
      },
      {
        id: 203,
        catId: 'phi-hoa-3d',
        catName: 'Đèn lồng phi hoa 3D',
        name: 'Đèn lồng phi hoa 3D kiểu bánh ú & kim cương',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An_4.jpg?width=600',
        desc: 'Dáng bánh ú và kim cương bọc vải phi hoa 3D bền màu, khung tre chắc chắn.'
      },
      {
        id: 204,
        catId: 'phi-hoa-3d',
        catName: 'Đèn lồng phi hoa 3D',
        name: 'Đèn lồng nhí Hội An vải phi hoa trang trí cây & tiểu cảnh',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Hoi_An_lanterns.jpg?width=600',
        desc: 'Đèn lồng Hội An mini 10cm - 20cm vải phi hoa nhiều màu dùng treo cây, làm rèm và trang trí tiểu cảnh Tết.'
      },

      // Nhóm 3: Vải hoa & Gấm trúc
      {
        id: 301,
        catId: 'vai-hoa-gam-truc',
        catName: 'Vải hoa & Gấm trúc',
        name: 'Đèn lồng vải gấm trúc Hội An hoa văn cổ điển',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lantern_Shop_in_Hoi_An_1.jpg?width=600',
        desc: 'Chất liệu vải gấm dệt họa tiết tùng trúc, chữ Thọ, hoa mẫu đơn cổ điển mang đậm phong cách truyền thống Hội An.'
      },
      {
        id: 302,
        catId: 'vai-hoa-gam-truc',
        catName: 'Vải hoa & Gấm trúc',
        name: 'Đèn tre truyền thống bọc vải bành hoa trang trí nhà hàng',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lantern_Shop_in_Hoi_An_2.jpg?width=600',
        desc: 'Đèn lồng khung tre xử lý mối mọt bọc vải bành hoa họa tiết hoa cỏ tươi sáng, kích thước từ 30cm đến 100cm.'
      },

      // Nhóm 4: Xô Voan & Thổ cẩm
      {
        id: 401,
        catId: 'xo-voan-tho-cam',
        catName: 'Xô Voan & Thổ cẩm',
        name: 'Đèn lồng Xô Voan xuyên sáng dịu nhẹ decor phòng & spa',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lanterns_in_Hoi_An_5.jpg?width=600',
        desc: 'Chất liệu vải xô voan mềm mại, tán sáng êm dịu thích hợp decor phòng trà, spa, resort và studio.'
      },
      {
        id: 402,
        catId: 'xo-voan-tho-cam',
        catName: 'Xô Voan & Thổ cẩm',
        name: 'Bộ đèn lồng thổ cẩm Hội An 35cm trang trí độc đáo',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/The_obligatory_(yet_pretty)_lanterns_(14488457328).jpg?width=600',
        desc: 'Đèn lồng bọc vải thổ cẩm dệt hoa văn truyền thống kết hợp khung tre già uốn thủ công tỉ mỉ.'
      },

      // Nhóm 5: Thêu tay & Vẽ họa tiết
      {
        id: 501,
        catId: 'theu-tay-ve-hoa-tiet',
        catName: 'Thêu tay & Vẽ họa tiết',
        name: 'Đèn lồng lụa vẽ tay hoa đào, hoa sen & phố cổ Hội An',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Hoi_An_lantern_lights_(39513532072).jpg?width=600',
        desc: 'Nghệ nhân xưởng Hạnh Đào vẽ tay trực tiếp lên lụa tơ tằm: Hoa đào, hoa mai, hoa sen, cá chép, Chùa Cầu và phố cổ Hội An.'
      },
      {
        id: 502,
        catId: 'theu-tay-ve-hoa-tiet',
        catName: 'Thêu tay & Vẽ họa tiết',
        name: 'Đèn lồng đĩa bay & củ tỏi thêu hoa văn nghệ thuật',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lantern_Shop_in_H%E1%BB%99i_An_(4251657582).jpg?width=600',
        desc: 'Đèn lồng thêu tay và vẽ tranh phong cảnh tạo hiệu ứng ánh sáng sang trọng khi treo cao.'
      },

      // Nhóm 6: In Logo & Sự kiện
      {
        id: 601,
        catId: 'in-logo-su-kien',
        catName: 'Đèn lồng in Logo',
        name: 'Đèn lồng đỏ in Logo thương hiệu nhà hàng, quán cà phê',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Chinese_New_Year_(Tet_Festival)_Lampion.jpg?width=600',
        desc: 'Nhận in logo, tên quán, câu chúc lên đèn lồng Hội An sắc nét theo yêu cầu, chiết khấu cao cho đơn hàng sỉ & dự án.'
      },
      {
        id: 602,
        catId: 'in-logo-su-kien',
        catName: 'Đèn lồng in Logo',
        name: 'Đèn lồng Hội An cỡ lớn trang trí sự kiện, lễ hội & Tết',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/H%E1%BB%99i_An_lantern_festival_(45485644722).jpg?width=600',
        desc: 'Chuyên sản xuất đèn lồng cỡ lớn 80cm, 1m, 1m2, 1m5 trang trí sảnh trung tâm thương mại, đường phố và lễ hội.'
      },

      // Nhóm 7: Đèn tre, Gỗ & Hoa sen
      {
        id: 701,
        catId: 'den-go-hoa-sen',
        catName: 'Đèn tre, Gỗ & Hoa sen',
        name: 'Lồng đèn tre đan tự nhiên Hạnh Đào Hội An thủ công tỉ mỉ',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Making_lanterns_in_Hoi_An_(31477021917).jpg?width=600',
        desc: 'Lồng đèn chất liệu tre tự nhiên đan thủ công trực tiếp tại Cơ Sở Sản Xuất Lồng Đèn Hạnh Đào – 92 Nguyễn Du, Hội An.'
      },
      {
        id: 702,
        catId: 'den-go-hoa-sen',
        catName: 'Đèn tre, Gỗ & Hoa sen',
        name: 'Đèn lồng hoa sen & Đèn gỗ lục giác trang trí phòng thờ, lễ Phật Đản',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Lotus_Lantern_Seoul_Lantern_Festival.jpg?width=600',
        desc: 'Đèn hoa sen vải nhăn cao cấp và đèn gỗ lục giác chạm khắc truyền thống.'
      },

      // Nhóm 8: Đèn lồng kiểu Nhật
      {
        id: 801,
        catId: 'den-long-nhat',
        catName: 'Đèn lồng kiểu Nhật',
        name: 'Đèn lồng kiểu Nhật dáng trụ dài trang trí nhà hàng Nhật',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/Paper_lantern.jpg?width=600',
        desc: 'Đèn lồng kiểu Nhật (Chochin) dáng trụ tròn và bầu dục, nhận vẽ chữ Kanji, hoa anh đào Sakura và in logo quán Izakaya.'
      },
      {
        id: 802,
        catId: 'den-long-nhat',
        catName: 'Đèn lồng kiểu Nhật',
        name: 'Đèn lồng tre kiểu Nhật & Hội An trang trí ngoài trời',
        price: 'Giá xưởng: Liên hệ 0796.693.304',
        image: 'https://commons.wikimedia.org/wiki/Special:FilePath/%C4%90%C3%A8n_l%E1%BB%93ng_H%E1%BB%99i_An_v%E1%BB%81_%C4%91%C3%AAm.jpg?width=600',
        desc: 'Mẫu đèn lồng chống thấm trang trí sân vườn, lối đi, suối nước nóng và nhà hàng phong cách Á Đông.'
      }
    ];

    let activeCategory = 'all';

    // Hàm render danh mục ra giao diện (cả 8 ô danh mục trên máy tính & điện thoại)
    function renderCategories() {
      const grid = document.getElementById('category-visual-grid');
      const pills = document.getElementById('category-pills');
      if (!grid || !pills) return;

      // Render 8 ô hình tròn/vuông danh mục trên trang chủ
      let htmlGrid = `
        <div onclick="filterByCategory('all')" class="cat-box cursor-pointer text-center group">
          <div class="w-16 h-16 sm:w-20 sm:h-20 md:w-24 md:h-24 mx-auto rounded-full overflow-hidden border-2 ${activeCategory === 'all' ? 'border-brand-red shadow-md scale-105' : 'border-stone-200'} bg-white transition">
            <img src="https://commons.wikimedia.org/wiki/Special:FilePath/Hoi_An_lantern_lampion_(38834258624).jpg?width=300" alt="Tất cả" class="w-full h-full object-cover">
          </div>
          <span class="block mt-1.5 text-[11px] sm:text-xs font-semibold ${activeCategory === 'all' ? 'text-brand-red font-bold' : 'text-stone-800'} line-clamp-2">Tất cả sản phẩm</span>
        </div>
      `;

      categories.forEach(cat => {
        const isActive = activeCategory === cat.id;
        htmlGrid += `
          <div onclick="filterByCategory('${cat.id}')" class="cat-box cursor-pointer text-center group">
            <div class="w-16 h-16 sm:w-20 sm:h-20 md:w-24 md:h-24 mx-auto rounded-full overflow-hidden border-2 ${isActive ? 'border-brand-red shadow-md scale-105' : 'border-stone-200'} bg-white transition">
              <img src="${cat.image}" alt="${cat.name}" class="w-full h-full object-cover">
            </div>
            <span class="block mt-1.5 text-[11px] sm:text-xs font-semibold ${isActive ? 'text-brand-red font-bold' : 'text-stone-800'} line-clamp-2">${cat.shortName}</span>
          </div>
        `;
      });
      grid.innerHTML = htmlGrid;

      // Render các nút lọc nhanh ngang
      let htmlPills = `
        <button onclick="filterByCategory('all')" class="px-3.5 py-1.5 rounded-full text-xs font-semibold whitespace-nowrap transition ${activeCategory === 'all' ? 'bg-brand-red text-white shadow' : 'bg-white text-stone-700 border border-stone-200 hover:bg-stone-100'}">
          Tất cả sản phẩm
        </button>
      `;
      categories.forEach(cat => {
        const isActive = activeCategory === cat.id;
        htmlPills += `
          <button onclick="filterByCategory('${cat.id}')" class="px-3.5 py-1.5 rounded-full text-xs font-semibold whitespace-nowrap transition ${isActive ? 'bg-brand-red text-white shadow' : 'bg-white text-stone-700 border border-stone-200 hover:bg-stone-100'}">
            ${cat.name}
          </button>
        `;
      });
      pills.innerHTML = htmlPills;
    }

    // Hàm render danh sách sản phẩm theo dạng Section chuẩn Flatsome (2 cột trên điện thoại, 4 cột trên máy tính)
    function renderProducts(keyword = '') {
      const wrapper = document.getElementById('product-sections-wrapper');
      if (!wrapper) return;

      let filtered = products;
      if (activeCategory !== 'all') {
        filtered = products.filter(p => p.catId === activeCategory);
      }

      if (keyword.trim() !== '') {
        const kw = keyword.toLowerCase();
        filtered = filtered.filter(p => p.name.toLowerCase().includes(kw) || p.desc.toLowerCase().includes(kw));
      }

      if (filtered.length === 0) {
        wrapper.innerHTML = `
          <div class="text-center py-12 bg-white rounded-2xl border border-stone-200 shadow-sm">
            <i class="fa-solid fa-box-open text-3xl text-stone-400 mb-2"></i>
            <p class="text-sm font-semibold text-stone-700">Không tìm thấy mẫu đèn lồng phù hợp.</p>
            <button onclick="filterByCategory('all'); document.getElementById('desktop-search').value='';" class="mt-3 px-4 py-2 bg-brand-red text-white text-xs rounded-full font-medium">Xem tất cả sản phẩm</button>
          </div>
        `;
        return;
      }

      // Nếu đang lọc theo danh mục cụ thể hoặc tìm kiếm
      if (activeCategory !== 'all' || keyword.trim() !== '') {
        const catObj = categories.find(c => c.id === activeCategory);
        const titleText = keyword.trim() !== '' ? `Kết quả tìm kiếm: "${keyword}"` : (catObj ? catObj.name : 'Sản phẩm đèn lồng');
        
        let html = `
          <div class="space-y-4">
            <div class="flex items-center justify-between border-b border-stone-200 pb-3">
              <h2 class="font-serif font-bold text-lg md:text-xl text-brand-red uppercase">${titleText}</h2>
              <span class="text-xs text-stone-500 font-medium">Hiển thị ${filtered.length} mẫu</span>
            </div>
            <div class="grid grid-cols-2 lg:grid-cols-4 gap-3 sm:gap-5">
        `;

        filtered.forEach(p => {
          html += generateProductCard(p);
        });

        html += `</div></div>`;
        wrapper.innerHTML = html;
        return;
      }

      // Trang chủ tổng hợp: Hiển thị đầy đủ từng section cho từng danh mục để trưng bày nhiều sản phẩm ra ngoài
      let htmlSections = '';
      categories.forEach(cat => {
        const catProducts = products.filter(p => p.catId === cat.id);
        if (catProducts.length === 0) return;

        htmlSections += `
          <div class="space-y-4 mb-10">
            <div class="flex items-center justify-between border-b border-stone-200 pb-2.5">
              <div class="flex items-center gap-2">
                <i class="fa-solid fa-lantern text-brand-red"></i>
                <h2 class="font-serif font-bold text-base md:text-xl text-brand-red uppercase tracking-wide">${cat.name}</h2>
              </div>
              <button onclick="filterByCategory('${cat.id}')" class="text-xs font-semibold text-brand-red hover:underline flex items-center gap-1">
                <span>Xem tất cả</span>
                <i class="fa-solid fa-angle-right"></i>
              </button>
            </div>
            <div class="grid grid-cols-2 lg:grid-cols-4 gap-3 sm:gap-5">
        `;

        catProducts.forEach(p => {
          htmlSections += generateProductCard(p);
        });

        htmlSections += `</div></div>`;
      });

      wrapper.innerHTML = htmlSections;
    }

    // Helper tạo thẻ sản phẩm chuẩn Flatsome (2 cột trên điện thoại, 4 cột trên máy tính, KHÔNG CÓ NHÃN DÁN)
    function generateProductCard(p) {
      return `
        <div class="product-box bg-white rounded-xl overflow-hidden border border-stone-200/80 shadow-sm hover:shadow-md transition flex flex-col justify-between group">
          <div>
            <div class="box-image w-full h-44 sm:h-56 bg-stone-100 relative cursor-pointer" onclick="openProductModal(${p.id})">
              <img src="${p.image}" alt="${p.name}" class="w-full h-full object-cover" onerror="this.src='https://placehold.co/400x400/9E1B1B/ffffff?text=Long+Den+Hanh+Dao'">
            </div>
            <div class="p-3 sm:p-4 space-y-1.5">
              <span class="text-[10px] uppercase font-semibold text-stone-400 tracking-wider block">${p.catName}</span>
              <h3 onclick="openProductModal(${p.id})" class="font-semibold text-xs sm:text-sm text-stone-800 line-clamp-2 hover:text-brand-red cursor-pointer transition leading-snug">
                ${p.name}
              </h3>
            </div>
          </div>
          <div class="p-3 sm:p-4 pt-0 space-y-2.5">
            <div class="text-xs sm:text-sm font-bold text-brand-red">${p.price}</div>
            <div class="grid grid-cols-2 gap-1.5">
              <button onclick="openProductModal(${p.id})" class="py-1.5 px-2 rounded-lg bg-stone-100 hover:bg-stone-200 text-stone-800 text-[11px] font-semibold transition text-center">
                Chi tiết
              </button>
              <a href="https://zalo.me/0796693304" target="_blank" rel="noopener noreferrer" class="py-1.5 px-2 rounded-lg bg-brand-red hover:bg-brand-darkRed text-white text-[11px] font-semibold transition text-center flex items-center justify-center gap-1">
                <i class="fa-solid fa-phone"></i> Đặt mua
              </a>
            </div>
          </div>
        </div>
      `;
    }

    // Lọc theo danh mục
    function filterByCategory(catId) {
      activeCategory = catId;
      renderCategories();
      renderProducts();
      // Cuộn mượt đến phần sản phẩm
      const section = document.getElementById('san-pham');
      if (section && catId !== 'all') {
        section.scrollIntoView({ behavior: 'smooth' });
      }
    }

    // Xử lý tìm kiếm
    function handleSearch(val) {
      renderProducts(val);
    }

    // Modal chi tiết sản phẩm
    function openProductModal(productId) {
      const p = products.find(item => item.id === productId);
      if (!p) return;

      document.getElementById('modal-img').src = p.image;
      document.getElementById('modal-cat').innerText = p.catName;
      document.getElementById('modal-title').innerText = p.name;
      document.getElementById('modal-price').innerText = p.price;
      document.getElementById('modal-desc').innerText = p.desc;

      const modal = document.getElementById('product-modal');
      modal.classList.remove('hidden');
      modal.classList.add('flex');
    }

    function closeProductModal() {
      const modal = document.getElementById('product-modal');
      modal.classList.remove('flex');
      modal.classList.add('hidden');
    }

    // Slider tự trượt 2 ảnh banner
    let currentSlide = 0;
    const totalSlides = 2;
    let slideInterval;

    function showSlide(index) {
      const slides = document.querySelectorAll('.hero-slide');
      slides.forEach((slide, i) => {
        if (i === index) {
          slide.classList.remove('opacity-0', 'z-0');
          slide.classList.add('opacity-100', 'z-10');
        } else {
          slide.classList.remove('opacity-100', 'z-10');
          slide.classList.add('opacity-0', 'z-0');
        }
      });

      for (let i = 0; i < totalSlides; i++) {
        const dot = document.getElementById(`dot-${i}`);
        if (dot) {
          if (i === index) {
            dot.className = 'w-7 h-2 rounded-full bg-amber-400 transition-all';
          } else {
            dot.className = 'w-2.5 h-2 rounded-full bg-white/60 transition-all';
          }
        }
      }
      currentSlide = index;
    }

    function changeSlide(direction) {
      let next = currentSlide + direction;
      if (next >= totalSlides) next = 0;
      if (next < 0) next = totalSlides - 1;
      showSlide(next);
      resetTimer();
    }

    function goToSlide(index) {
      showSlide(index);
      resetTimer();
    }

    function resetTimer() {
      clearInterval(slideInterval);
      slideInterval = setInterval(() => {
        let next = currentSlide + 1;
        if (next >= totalSlides) next = 0;
        showSlide(next);
      }, 4500);
    }

    // Toggle menu điện thoại
    function toggleMobileMenu() {
      const drawer = document.getElementById('mobile-menu-drawer');
      const backdrop = document.getElementById('mobile-menu-backdrop');
      if (!drawer || !backdrop) return;

      if (drawer.classList.contains('-translate-x-full')) {
        drawer.classList.remove('-translate-x-full');
        backdrop.classList.remove('hidden');
      } else {
        drawer.classList.add('-translate-x-full');
        backdrop.classList.add('hidden');
      }
    }

    // Gửi yêu cầu báo giá nhanh
    function submitQuickQuote(e) {
      e.preventDefault();
      const name = document.getElementById('quote-name').value;
      const phone = document.getElementById('quote-phone').value;
      const successEl = document.getElementById('quote-success');
      successEl.innerText = `Cảm ơn ${name}! Yêu cầu báo giá của bạn đã được gửi đến xưởng Hạnh Đào. Chúng tôi sẽ liên hệ lại qua số ${phone} ngay!`;
      successEl.classList.remove('hidden');
      e.target.reset();
      setTimeout(() => {
        successEl.classList.add('hidden');
      }, 6000);
    }

    // Khởi chạy khi trang tải xong
    window.onload = function() {
      renderCategories();
      renderProducts();
      slideInterval = setInterval(() => {
        let next = currentSlide + 1;
        if (next >= totalSlides) next = 0;
        showSlide(next);
      }, 4500);
    };
  </script>
</body>
</html>
