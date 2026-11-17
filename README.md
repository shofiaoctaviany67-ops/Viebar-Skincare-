<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>LUMIERE - Toko Skincare</title>
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Arial,sans-serif}
header{background:#FF8FA3;color:#fff;padding:20px;text-align:center}
nav{background:#333;padding:12px;text-align:center}
nav a{color:#fff;margin:0 12px;text-decoration:none;font-weight:bold}
.hero{background:#FFE8EE;padding:40px 20px;text-align:center}
.hero h1{font-size:32px}
.hero button{padding:12px 24px;background:#111;color:#fff;border:none;border-radius:20px;margin-top:15px}
.container{padding:20px;max-width:900px;margin:auto}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:15px}
.card{background:#fff;border:1px solid #eee;border-radius:15px;overflow:hidden;box-shadow:0 3px 10px rgba(0,0,0,.1)}
.card img{width:100%;height:200px;object-fit:cover}
.card-body{padding:15px}
.price{color:#E91E63;font-weight:bold;margin:8px 0}
.btn{width:100%;padding:10px;background:#25D366;border:none;color:#fff;border-radius:10px;font-weight:bold;cursor:pointer}
footer{background:#111;color:#fff;text-align:center;padding:20px;margin-top:20px}
</style>
</head>
<body>

<header><h1>LUMIERE Skincare ✨</h1><p>Skincare Aman, BPOM & Halal</p></header>
<nav><a href="#">Beranda</a><a href="#produk">Produk</a><a href="#tentang">Tentang</a></nav>

<div class="hero">
<h1>Kulit Glowing, Percaya Diri Meningkat!</h1>
<p>Diskon 20% untuk pembelian pertama. Gratis ongkir!</p>
<button onclick="alert('Selamat datang di LUMIERE!')">Belanja Sekarang</button>
</div>

<div class="container" id="produk">
<h2>Produk Kami</h2><br>
<div class="grid">
<div class="card">
<img src="https://images.unsplash.com/photo-1620916566398-39f1143ab7be?w=500">
<div class="card-body"><h3>Brightening Serum</h3><p>Vitamin C + Niacinamide untuk cerahkan kulit.</p><div class="price">Rp 129.000</div><button class="btn" onclick="beli('Brightening Serum')">Beli</button></div>
</div>
<div class="card">
<img src="https://images.unsplash.com/photo-1556228720-195a672e8a03?w=500">
<div class="card-body"><h3>Facial Wash Gentle</h3><p>pH 5.5, lembut untuk kulit sensitif.</p><div class="price">Rp 59.000</div><button class="btn" onclick="beli('Facial Wash')">Beli</button></div>
</div>
<div class="card">
<img src="https://images.unsplash.com/photo-1570172619644-dfd03ed5d881?w=500">
<div class="card-body"><h3>Moisturizer Gel</h3><p>Hyaluronic Acid, lembab 24 jam.</p><div class="price">Rp 89.000</div><button class="btn" onclick="beli('Moisturizer')">Beli</button></div>
</div>
</div>
</div>

<div class="container" id="tentang">
<h2>Tentang Kami</h2>
<p style="margin-top:10px;line-height:1.6">LUMIERE adalah toko skincare lokal yang menjual produk aman, sudah BPOM, dan halal. Kami membantu remaja dan dewasa mendapatkan kulit sehat dan glowing tanpa merkuri.</p>
<p style="margin-top:10px"><b>Visi:</b> Menjadi brand skincare No.1 di Indonesia.<br><b>Misi:</b> Memberikan skincare berkualitas dengan harga terjangkau.</p>
</div>

<div class="container">
<h2>Keranjang: <span id="count">0</span> produk</h2>
<p id="list">Belum ada produk.</p>
</div>

<footer><p>© 2026 LUMIERE - Dibuat untuk Tugas Sekolah | IG: @lumiere.id | WA: 0812-3456-7890</p></footer>

<script>
let cart=[];
function beli(nama){cart.push(nama);document.getElementById('count').innerText=cart.length;document.getElementById('list').innerText='Kamu membeli: '+cart.join(', ');alert(nama+' ditambahkan!')}
</script>
</body>
</html>
