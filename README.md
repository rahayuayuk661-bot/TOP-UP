# TOP-UP
top up all games
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Roblox Top Up | Fast & Trusted</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
  <h1>ROBLOX TOP UP</h1>
  <p>Fast • Trusted • Dark Premium</p>
</header>

<section class="card">
  <h2>Top Up Robux</h2>

  <label>Username Roblox</label>
  <input type="text" id="username" placeholder="Contoh: Player123">

  <label>Pilih Nominal</label>
  <select id="nominal">
    <option value="80 Robux">80 Robux</option>
    <option value="400 Robux">400 Robux</option>
    <option value="800 Robux">800 Robux</option>
    <option value="1700 Robux">1700 Robux</option>
  </select>

  <button onclick="orderWA()">ORDER VIA WHATSAPP</button>
</section>

<footer>
  © 2026 Roblox Top Up
</footer>

<script src="script.js"></script>
</body>
</html>
body {
  margin: 0;
  font-family: Poppins, Arial, sans-serif;
  background: #0b0f19;
  color: #e5e7eb;
}

header {
  text-align: center;
  padding: 40px 20px;
}

header h1 {
  color: #6366f1;
  margin-bottom: 5px;
}

.card {
  max-width: 400px;
  background: #111827;
  margin: auto;
  padding: 25px;
  border-radius: 14px;
  box-shadow: 0 0 30px rgba(99,102,241,0.25);
}

label {
  display: block;
  margin-top: 15px;
  font-size: 14px;
}

input, select {
  width: 100%;
  padding: 12px;
  margin-top: 6px;
  border-radius: 8px;
  border: none;
  background: #1f2933;
  color: #ffffff;
}

button {
  width: 100%;
  margin-top: 25px;
  padding: 14px;
  background: linear-gradient(90deg,#6366f1,#4f46e5);
  border: none;
  border-radius: 10px;
  color: white;
  font-size: 16px;
  cursor: pointer;
}

button:hover {
  opacity: 0.9;
}

footer {
  text-align: center;
  margin: 40px 0;
  font-size: 13px;
  color: #9ca3af;
}
function orderWA() {
  const user = document.getElementById("username").value;
  const nominal = document.getElementById("nominal").value;

  if (user === "") {
    alert("Masukkan Username Roblox");
    return;
  }

  const nomor = "6281327759544";
  const pesan = `Halo Admin, saya ingin Top Up Roblox\nUsername: ${user}\nNominal: ${nominal}`;

  window.open(`https://wa.me/${nomor}?text=${encodeURIComponent(pesan)}`);
}
