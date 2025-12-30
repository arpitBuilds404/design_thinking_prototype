<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>EV Charge Network – Prototype</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
<style>
*{box-sizing:border-box;font-family:Inter}
body{margin:0;background:#f4f6f8}
header{
  background:#0b3c5d;color:#fff;padding:14px 30px;
  display:flex;justify-content:space-between;align-items:center
}
header h2{margin:0;font-size:20px}
nav a{color:#fff;margin-left:20px;text-decoration:none;font-size:14px}

.container{max-width:1100px;margin:30px auto;padding:20px}

.card{
  background:#fff;border-radius:14px;padding:24px;
  box-shadow:0 10px 30px rgba(0,0,0,.08);
  margin-bottom:30px
}

h3{margin-top:0}
.btn{
  background:#0a7cff;color:#fff;border:none;
  padding:12px 22px;border-radius:10px;
  font-size:15px;cursor:pointer
}
.btn.green{background:#00a86b}
.badge{background:#eef5ff;color:#0a7cff;padding:6px 12px;border-radius:20px;font-size:12px}

.grid{display:grid;grid-template-columns:1fr 1fr;gap:20px}
input,select{
  width:100%;padding:12px;border-radius:10px;
  border:1px solid #ddd;margin-top:8px
}

.map{
  height:260px;border-radius:14px;
  background:linear-gradient(135deg,#cfe7ff,#e8f3ff);
  display:flex;align-items:center;justify-content:center;
  color:#0b3c5d;font-weight:600
}

.payment img{height:34px;margin-right:15px}
.footer{text-align:center;color:#777;font-size:13px}
</style>
</head>

<body>

<header>
  <h2>⚡ EV Charge Network</h2>
  <nav>
    <a href="#">Find Chargers</a>
    <a href="#">Host</a>
    <a href="#">Contact</a>
  </nav>
</header>

<div class="container">

<!-- LOGIN -->
<div class="card">
  <h3>Login</h3>
  <div class="grid">
    <div>
      <label>Email / Phone</label>
      <input placeholder="Enter email or phone">
    </div>
    <div>
      <label>Password</label>
      <input type="password" placeholder="Password">
    </div>
  </div>
  <br>
  <button class="btn">Login</button>
  <span class="badge">Driver / Host</span>
</div>

<!-- MAP -->
<div class="card">
  <h3>Nearby Chargers</h3>
  <div class="map">Live Charger Map (Prototype)</div>
</div>

<!-- CHARGER DETAILS -->
<div class="card">
  <h3>Charger Details</h3>
  <p><b>Location:</b> Sector 21, Noida</p>
  <p><b>Speed:</b> 7.4 kW AC</p>
  <p><b>Price:</b> ₹12 / unit</p>
  <p><b>Status:</b> Available</p>
  <button class="btn green">Request Slot</button>
</div>

<!-- PAYMENT -->
<div class="card">
  <h3>Payment</h3>
  <p><b>Amount:</b> ₹250</p>
  <div class="payment">
    <img src="https://upload.wikimedia.org/wikipedia/commons/5/5e/Paytm_logo.png">
    <img src="https://upload.wikimedia.org/wikipedia/commons/f/f2/Google_Pay_Logo.svg">
    <img src="https://upload.wikimedia.org/wikipedia/commons/7/7b/BHIM_UPI_Logo.png">
  </div>
  <br>
  <button class="btn">Pay Now</button>
  <p class="badge">🔒 100% Secure Payment</p>
</div>

<!-- HOST DASHBOARD -->
<div class="card">
  <h3>Host Dashboard</h3>
  <div class="grid">
    <div>
      <label>Charger Type</label>
      <select>
        <option>AC</option>
        <option>DC Fast</option>
      </select>
    </div>
    <div>
      <label>Price per unit</label>
      <input placeholder="₹">
    </div>
  </div>
  <br>
  <button class="btn green">Add Charger</button>
</div>

<div class="footer">
  Prototype only • Backend not implemented • EV Charge Network
</div>

</div>
</body>
</html>
