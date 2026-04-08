# Kenya-chicken-<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kenyan Chicken 🐔 | Poultry Business</title>

<style>
*{
  box-sizing:border-box;
}
body{
  margin:0;
  font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Arial;
  background:#eef1f4;
  color:#1c1e21;
}
.topbar{
  background:#1877f2;
  color:#fff;
  padding:16px;
  font-size:22px;
  font-weight:700;
  position:sticky;
  top:0;
  function showSection(section) {
    document.querySelectorAll('.content').forEach(sec => {
        sec.classList.add('hidden');
    });
    document.getElementById(section).classList.remove('hidden');
}

function addPost() {
    const title = document.getElementById('title').value;
    const content = document.getElementById('content').value;
    const category = document.getElementById('category').value;

    if (!title || !content) {
        alert("Please fill all fields");
        return;
    }

    const postDiv = document.createElement('div');
    postDiv.innerHTML = `<h3>${title}</h3><p>${content}</p><hr>`;

    document.getElementById(category + "Posts").appendChild(postDiv);

    document.getElementById('title').value = "";
    document.getElementById('content').value = "";
}
  z-index:100;
  text-align:center;
}
.container{
  max-width:650px;
  margin:auto;
  padding:12px;
}
.card{
  background:#fff;
  border-radius:12px;
  margin-bottom:16px;
  box-shadow:0 2px 8px rgba(0,0,0,0.08);
  overflow:hidden;
}
.card-header{
  padding:12px;
  display:flex;
  align-items:center;
  gap:10px;
  font-weight:600;
}
.avatar{
  width:40px;
  height:40px;
  border-radius:50%;
  background:#ddd;
}
.card img{
  width:100%;
  display:block;
}
.card-body{
  padding:14px;
  font-size:15px;
  line-height:1.5;
}
.badge{
  display:inline-block;
  background:#e7f3ff;
  color:#1877f2;
  padding:4px 10px;
  border-radius:20px;
  font-size:13px;
  margin-top:6px;
}
.list{
  padding-left:20px;
}
.list li{
  margin-bottom:6px;
}
.footer{
  background:#fff;
  padding:18px;
  text-align:center;
  font-size:14px;
  color:#555;
}
.whatsapp{
  position:fixed;
  right:18px;
  bottom:18px;
  background:#25d366;
  color:white;
  padding:14px 20px;
  border-radius:40px;
  text-decoration:none;
  font-weight:700;
  box-shadow:0 6px 12px rgba(0,0,0,0.25);
}
.trust{
  display:flex;
  justify-content:space-around;
  padding:12px 0;
  font-size:13px;
  background:#f7f7f7;
}
.trust div{
  text-align:center;
}
</style>
</head>

<body>

<div class="topbar">Kenyan Chicken 🐔</div>

<div class="container">

  <!-- INTRO -->
  <div class="card">
    <div class="card-header">
      <div class="avatar"></div>
      Kenyan Chicken 🐔
    </div>
    <img src="https://images.unsplash.com/photo-1548550023-2bdb3c5beed7">
    <div class="card-body">
      We are a Kenyan-based poultry business specializing in
      <b>kienyeji</b> and <b>broiler</b> chickens.
      Healthy birds, proper feeding, and reliable supply.
      <div class="badge">Trusted Poultry Business</div>
    </div>
  </div>

  <!-- EGGS -->
  <div class="card">
    <div class="card-header">
      <div class="avatar"></div>
      Fresh Eggs 🥚
    </div>
    <img src="https://images.unsplash.com/photo-1587486913049-53fc88980cfc">
    <div class="card-body">
      Fresh kienyeji eggs available daily.
      Clean, well handled, and suitable for home or commercial use.
      <div class="badge">Retail & Bulk Orders</div>
    </div>
  </div>

  <!-- SERVICES -->
  <div class="card">
    <div class="card-header">
      <div class="avatar"></div>
      Our Services
    </div>
    <img src="https://images.unsplash.com/photo-1604908177522-429e3c8b0a36">
    <div class="card-body">
      <ul class="list">
        <li>Chicken rearing (kienyeji & broiler)</li>
        <li>Egg supply</li>
        <li>Bulk orders</li>
        <li>Farmer support & guidance</li>
      </ul>
    </div>
  </div>

  <!-- LOCATION -->
  <div class="card">
    <div class="card-header">
      <div class="avatar"></div>
      Location & Orders
    </div>
    <div class="card-body">
      📍 Kenya <br>
      📞 Call or WhatsApp to place orders <br>
      🚚 Delivery available (location based)
    </div>
    <div class="trust">
      <div>✔ Real Business</div>
      <div>✔ Kenya Based</div>
      <div>✔ Direct Orders</div>
    </div>
  </div>

</div>

<div class="footer">
  © 2025 Kenyan Chicken 🐔 <br>
  Poultry you can trust
</div>

<a class="whatsapp" href="https://wa.me/254700000000">WhatsApp</a>

</body>
</html>
