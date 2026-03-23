<!DOCTYPE html>
<html>
<head>
<title>Aqua Fresh Karachi</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<!-- Icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
body {
  margin: 0;
  font-family: Arial;
  background: #f4fbff;
}

header {
  background: #0077b6;
  color: white;
  padding: 15px;
  text-align: center;
}

.logo {
  max-width: 180px;
}

.banner {
  background: linear-gradient(to right, #00b4d8, #0077b6);
  color: white;
  text-align: center;
  padding: 50px 20px;
}

.section {
  padding: 30px;
  text-align: center;
}

.cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.card {
  background: white;
  margin: 15px;
  padding: 20px;
  width: 250px;
  border-radius: 12px;
  box-shadow: 0 0 10px rgba(0,0,0,0.1);
  transition: 0.3s;
}

.card:hover {
  transform: scale(1.05);
}

.card i {
  font-size: 30px;
  color: #0077b6;
  margin-bottom: 10px;
}

.contact {
  background: #caf0f8;
  padding: 30px;
  text-align: center;
}

input {
  width: 80%;
  padding: 12px;
  border-radius: 6px;
  border: 1px solid #ccc;
}

button {
  background: #0077b6;
  color: white;
  padding: 12px 25px;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

button:hover {
  background: #023e8a;
}

footer {
  background: #0077b6;
  color: white;
  text-align: center;
  padding: 12px;
}

/* WhatsApp Button */
.whatsapp {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background: #25D366;
  color: white;
  padding: 12px 18px;
  border-radius: 50px;
  text-decoration: none;
  font-weight: bold;
  display: flex;
  align-items: center;
  gap: 8px;
}
</style>

</head>

<body>

<header>
  <img src="https://i.postimg.cc/5tMc8cy0/file-0000000099b871fa94281d031728d2e3.png" class="logo">
  <h2>Aqua Fresh Karachi</h2>
  <p>Pure & Safe Drinking Water</p>
</header>

<div class="banner">
  <h2>Clean & Healthy Water</h2>
  <p>RO Purified | UV & Ozone Treated</p>
</div>

<div class="section">
  <h2>Our Services</h2>

  <div class="cards">
    <div class="card">
      <i class="fas fa-tint"></i>
      <h3>RO Water</h3>
      <p>High quality drinking water</p>
    </div>

    <div class="card">
      <i class="fas fa-shield-virus"></i>
      <h3>UV Treatment</h3>
      <p>Advanced purification</p>
    </div>

    <div class="card">
      <i class="fas fa-truck"></i>
      <h3>Home Delivery</h3>
      <p>Fast delivery service</p>
    </div>
  </div>
</div>

<div class="contact">
  <h2>Order Now</h2>

  <form onsubmit="sendToWhatsApp(event)">
    <input type="text" id="name" placeholder="Your Name" required><br><br>
    <input type="text" id="phone" placeholder="Phone Number" required><br><br>
    <input type="text" id="address" placeholder="Address" required><br><br>
    <button type="submit">
      <i class="fas fa-paper-plane"></i> Submit Order
    </button>
  </form>

  <h3>Contact</h3>
  <p><i class="fas fa-user"></i> Malik Arshad</p>
  <p><i class="fas fa-phone"></i> 0300-2427705</p>
  <p><i class="fab fa-whatsapp"></i> WhatsApp Available</p>
</div>

<!-- Google Map -->
<iframe src="https://maps.google.com/maps?q=karachi&t=&z=13&ie=UTF8&iwloc=&output=embed"
width="100%" height="250"></iframe>

<footer>
  <p>© Aqua Fresh Karachi</p>
</footer>

<!-- WhatsApp Button -->
<a class="whatsapp" href="https://wa.me/923002427705" target="_blank">
  <i class="fab fa-whatsapp"></i> Chat Now
</a>

<!-- WhatsApp Order Script -->
<script>
function sendToWhatsApp(e) {
  e.preventDefault();

  let name = document.getElementById("name").value;
  let phone = document.getElementById("phone").value;
  let address = document.getElementById("address").value;

  let message = `New Order:%0AName: ${name}%0APhone: ${phone}%0AAddress: ${address}`;

  window.open(`https://wa.me/923002427705?text=${message}`, '_blank');
}
</script>

</body>
</html>
