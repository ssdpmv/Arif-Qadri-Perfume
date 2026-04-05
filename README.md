<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Arif Qadri Perfumes</title>

<style>
body {
    margin: 0;
    font-family: Arial;
    background: black;
    color: white;
    text-align: center;
}

h1 {
    padding: 20px;
}

.products {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px,1fr));
    gap: 20px;
    padding: 20px;
}

.card {
    background: #111;
    border-radius: 10px;
    padding: 15px;
}

button {
    background: gold;
    color: black;
    padding: 10px;
    border: none;
    margin-top: 10px;
    cursor: pointer;
    font-weight: bold;
}

button:hover {
    background: orange;
}
</style>
</head>

<body>

<h1>Arif Qadri Perfumes</h1>

<div class="products">

<div class="card">
<h3>Oud Royal</h3>
<p>₹999</p>
<button onclick="order('Oud Royal')">Buy Now</button>
</div>

<div class="card">
<h3>Rose Musk</h3>
<p>₹799</p>
<button onclick="order('Rose Musk')">Buy Now</button>
</div>

<div class="card">
<h3>Night Desire</h3>
<p>₹1199</p>
<button onclick="order('Night Desire')">Buy Now</button>
</div>

<div class="card">
<h3>Royal Attar</h3>
<p>₹699</p>
<button onclick="order('Royal Attar')">Buy Now</button>
</div>

</div>

<p>📞 Mob: YOUR_NUMBER</p>
<p>📧 Email: xyz@gmail.com</p>

<script>
function order(product){
let number = "91XXXXXXXXXX"; // apna number daalo
let msg = "I want to order " + product;
let url = "https://wa.me/" + number + "?text=" + encodeURIComponent(msg);
window.open(url, "_blank");
}
</script>

</body>
</html>
