 <!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Rayy Store</title>
  <style>
    /* CSS Variables */
    :root {
      --font-sans: 'Poppins', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      --color-bg: #ffffff;
      --color-primary: #1f2937; /* dark slate */
      --color-secondary: #4b5563; /* gray 600 */
      --color-accent: #3b82f6; /* blue 500 */
      --color-link-hover: #2563eb; /* blue 600 */
      --color-price: #10b981; /* emerald 500 */
      --border-radius: 0.75rem;
      --shadow-soft: 0 4px 6px rgba(0,0,0,0.1);
      --transition-speed: 0.3s;
    }

    /* Reset & base */
    * {
      box-sizing: border-box;
    }
    body {
      margin: 0;
      font-family: var(--font-sans);
      background-color: var(--color-bg);
      color: var(--color-primary);
      line-height: 1.5;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      font-size: 18px;
      padding: 2rem 1rem;
      display: flex;
      justify-content: center;
      min-height: 100vh;
    }

    main.container {
      max-width: 640px;
      width: 100%;
    }

    /* Text styles */
    h1 {
      font-size: 3rem;
      font-weight: 700;
      margin-bottom: 0.25rem;
      text-align: center;
      color: var(--color-primary);
    }

    h2 {
      font-size: 2rem;
      font-weight: 600;
      margin-top: 0;
      margin-bottom: 1.25rem;
      text-align: center;
      color: var(--color-secondary);
      font-style: italic;
    }

    p.description {
      text-align: center;
      color: var(--color-secondary);
      font-size: 1.125rem;
      margin-bottom: 2rem;
      user-select: none;
    }

    /* Product list */
    ul.product-list {
      list-style: none;
      padding: 0;
      margin: 0;
    }

    li.product-item {
      background: #f9fafb;
      margin-bottom: 1rem;
      border-radius: var(--border-radius);
      box-shadow: var(--shadow-soft);
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 1.5rem;
      transition: box-shadow var(--transition-speed), transform var(--transition-speed);
      cursor: pointer;
    }

    li.product-item:hover,
    li.product-item:focus-within {
      box-shadow: 0 8px 16px rgba(59, 130, 246, 0.3);
      transform: translateY(-2px);
    }

    a.product-link {
      text-decoration: none;
      color: var(--color-primary);
      font-weight: 600;
      font-size: 1.125rem;
      flex-grow: 1;
      outline-offset: 4px;
      transition: color var(--transition-speed);
    }

    a.rayystore.com:hover,
    a.rayystore.com:focus {
      color: var(--color-link-hover);
    }

    span.price {
      font-weight: 700;
      color: var(--color-price);
      flex-shrink: 0;
      margin-left: 1rem;
      font-size: 1.125rem;
      user-select: none;
    }

    /* Accessibility: focus visible */
    a.product-link:focus-visible,
    li.product-item:focus-visible {
      outline: 2px solid var(--color-accent);
      outline-offset: 2px;
    }

    /* Responsive tweaks */
    @media (max-width: 480px) {
      h1 {
        font-size: 2.25rem;
      }
      h2 {
        font-size: 1.5rem;
      }
      p.description {
        font-size: 1rem;
      }
    }
  </style>
</head>
<body>
  <main class="container" role="main" aria-label="Rayy Store product list">
    <h1>Selamat Datang</h1>
    <h2>Rayy Store</h2>
    <p class="description">Silakan Pilih Produk Yang Anda Mau, No Produk Sesuai Dengan Yang Di Deskripsi</p>
    <ul class="product-list" aria-label="Daftar produk">
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/60FjSAobk0" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product1">1. Hoodie Boxy Oversize Dizzy Moon</a>
        <span class="price">Rp 74.700</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/2qIhgTJu1m" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product2">2. Sepatu Sneakers Cool Putih/Hitam</a>
        <span class="price">Rp 115.000</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/4q3ka3V756?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product3">3. Jersey Persip Bandung Grade Ori</a>
        <span class="price">Rp 121.275</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/3LEwnWDdcv?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product4">4. Jersey Real Madrid Home Anak²</a>
        <span class="price">Rp 50.208</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/3LEwnWDdcv?share_channel_code=1"  class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">5. Jersey Real Madrid Home Dewasa</a>
        <span class="price">Rp 74.692</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href=https://s.shopee.co.id/2B30sf6K2Q class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">6. Jersey Timnas Indo Home/Away</a>
        <span class="price">Rp 109.781</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href=https://s.shopee.co.id/yWIuvNgC class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">7. Jersey Timnas Indo Away Lengan Panjang</a>
        <span class="price">Rp 123.330</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/qXbr2Zkjx?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">8. Sepatu Adidas F50</a>
        <span class="price">Rp 251.270</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/4Ao3pZpjkn?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">9. Sepatu  Adidas Predator</a>
        <span class="price">Rp 164.800</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/9KW9xxg8RM?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">10. Jersey Retro France</a>
        <span class="price">Rp Rp86.800</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/LbLFJv1qh?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">11. Jersey Retro Brazil</a>
        <span class="price">Rp 115.500</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/7ARfNkce7X?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">12. Retro Manchester U Home 1999</a>
        <span class="price">Rp 169.900</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/9zlqkbwXTv?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">12. Man United Retro 1998 Long Slevee</a>
        <span class="price">Rp 208.999</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/7fNvxqRzPv?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">13. Jersey Barcelona H/A/3rd Ori</a>
        <span class="price">Rp 244.000</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/9KWCkjskj8?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">14. Adidas Samba OG Putih Hitam</a>
        <span class="price">Rp 95.000</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/5L03zZ7jLY?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">15. Whitelab Facial Wash</a>
        <span class="price">Rp 43.000</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/20jc1zoxSk?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">16. Adidas Predator</a>
        <span class="price">Rp 149.400</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/1qQBpnM5kB?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">17. Skipping Skiping Alat Lompat Tali</a>
        <span class="price">Rp 66.500</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/AUiA9mwYam?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">18. TrailTop Handgrip Adjustable Strength 5~60KG</a>
        <span class="price">Rp 17.900</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/30c9E60LJq?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">19. WANNAFIT Pull Up Bar Door Chinning</a>
        <span class="price">Rp 72.000</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/2B32EedmqX?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">20. Spin Bike </a>
        <span class="price">Rp 955.000</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/qXeeMSvjw?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">21. SPEEDS Push Up Board Push Up  </a>
        <span class="price">Rp 104.400</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/1LTvFQo449?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">22. SPEEDS Gym Ball fitness 75 cm </a>
        <span class="price">Rp 57.200</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/60Fko5GbBp?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">24. Barbel Dumbel 1Kg </a>
        <span class="price">Rp 9.900</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/2LMSRPBktU?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">25. Treadmil, Twen T200 new</a>
        <span class="price">Rp 2.160.000</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/3frq1vMasS?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">26. Power Twister </a>
        <span class="price">Rp 57.500</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/4fkNDrCAaH?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">27. Apha Icarus </a>
        <span class="price">Rp 169.000</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/6fVRbcSnTM?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">28. SPECS Paket Komplit </a>
        <span class="price">Rp 87.000</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/8Ux5n2SvLm?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">29. Fromzero Starkia Baltic Putih Hitam </a>
        <span class="price">Rp 180.000</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/3LEzddom8G?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">30. Specs Ewaklok </a>
        <span class="price">Rp 249.000</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/30c9F61u1m?share_channel_code=1" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product5">31. Ortuseight EXTEND </a>
        <span class="price">Rp 299.500</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/5L08oOYFdY" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product32">32. Tas Ransel Cowo Bergambar 1</a>
        <span class="price">Rp 27.000</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/9UphmKFvCm" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product33">33. Tas Ransel Koduroy Bintang</a>
        <span class="price">Rp 99.000</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/800tzjUecq" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product34">34. Tas Ransel One Project Id</a>
        <span class="price">Rp 22.770</span>
      </li>
      <li class="product-item" tabindex="0">
        <a href="https://s.shopee.co.id/8KdkOQrQ6v" class="product-link" target="_blank" rel="noopener noreferrer" aria-describedby="desc-product35">35. Tas Ransel Corduroy Bintang II</a>
        <span class="price">Rp 94.500</span>
      </li>
    </ul>
  </main>
</body>
</html>
