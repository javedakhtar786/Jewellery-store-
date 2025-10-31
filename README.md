# Jewellery-store-
Jewellery store 
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>BRAND_NAME — Earrings & Rings</title>
  <style>
    body {font-family: Arial, sans-serif; margin:0; background:#f7f7f7;}
    header {background:#fff; padding:15px 20px; box-shadow:0 2px 5px rgba(0,0,0,0.1);}
    .brand {font-size:22px; font-weight:bold;}
    .tagline {color:#666; font-size:14px;}
    .container {max-width:1000px; margin:30px auto; padding:0 15px;}
    .grid {display:grid; grid-template-columns:repeat(auto-fit,minmax(220px,1fr)); gap:20px;}
    .card {background:#fff; border-radius:10px; padding:10px; box-shadow:0 2px 8px rgba(0,0,0,0.05);}
    .card img {width:100%; border-radius:8px;}
    h3 {margin:10px 0 5px;}
    .price {color:#d6455b; font-weight:bold;}
    .btn {display:inline-block; background:#d6455b; color:#fff; padding:8px 10px; text-decoration:none; border-radius:6px; font-size:14px;}
    footer {text-align:center; color:#777; padding:20px 0; font-size:14px;}
  </style>
</head>
<body>
  <header>
    <div class="brand">BRAND_NAME</div>
    <div class="tagline">Trendy Earrings & Rings Collection</div>
  </header>

  <div class="container">
    <h2>Our Collection</h2>
    <div class="grid">
      <div class="card" data-name="Oxidized Earrings">
        <img src="https://via.placeholder.com/300x200?text=Earring+1" alt="Oxidized Earrings">
        <h3>Oxidized Drop Earrings</h3>
        <p class="price">₹349</p>
        <a href="#" class="btn buy">Buy on WhatsApp</a>
      </div>

      <div class="card" data-name="Minimal Ring Set">
        <img src="https://via.placeholder.com/300x200?text=Ring+Set" alt="Ring Set">
        <h3>Minimal Ring Set</h3>
        <p class="price">₹399</p>
        <a href="#" class="btn buy">Buy on WhatsApp</a>
      </div>

      <div class="card" data-name="Pearl Hoop Earrings">
        <img src="https://via.placeholder.com/300x200?text=Earring+2" alt="Pearl Earrings">
        <h3>Pearl Hoop Earrings</h3>
        <p class="price">₹499</p>
        <a href="#" class="btn buy">Buy on WhatsApp</a>
      </div>
    </div>
  </div>

  <footer>
    © 2025 BRAND_NAME | Connect on WhatsApp
  </footer>

  <script>
    const WA_NUMBER = '919999999999'; // Replace with your WhatsApp number

    document.querySelectorAll('.buy').forEach(btn => {
      btn.addEventListener('click', e => {
        e.preventDefault();
        const product = e.target.closest('.card').dataset.name;
        const text = encodeURIComponent(`Hi, I'm interested in ${product}`);
        window.open(`https://wa.me/${WA_NUMBER}?text=${text}`, '_blank');
      });
    });
  </script>
</body>
</html>
