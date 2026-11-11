# J-GROOVE
Tienda de ropa urbana 


<!DOCTYPE html>

<html lang="es">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>J-GROOVE | Streetwear</title>

<style>

* {

  box-sizing: border-box;

  margin: 0;

  padding: 0;

}

body {

  background: #101510;

  color: #eee8d5;

  font-family: Arial, sans-serif;

}

header {

  background: #0b0e0b;

  padding: 22px 7%;

  display: flex;

  justify-content: space-between;

  align-items: center;

  border-bottom: 1px solid #294b34;

}

.logo {

  font-size: 27px;

  font-weight: 900;

  letter-spacing: 3px;

  color: #eee8d5;

}

.logo span {

  color: #438653;

}

nav a {

  color: #eee8d5;

  text-decoration: none;

  margin-left: 20px;

  font-size: 13px;

}

.hero {

  min-height: 440px;

  padding: 100px 8%;

  background: linear-gradient(90deg,#101510,#183d27);

  display: flex;

  flex-direction: column;

  justify-content: center;

}

.hero h1 {

  font-size: clamp(45px, 9vw, 85px);

  font-weight: 900;

  letter-spacing: -3px;

}

.hero h1 span {

  color: #65a477;

}

.hero p {

  margin-top: 18px;

  color: #c5c5b8;

  letter-spacing: 2px;

}

.hero a {

  display: inline-block;

  width: fit-content;

  margin-top: 30px;

  background: #eee8d5;

  color: #101510;

  padding: 15px 25px;

  text-decoration: none;

  font-weight: bold;

}

section {

  padding: 65px 7%;

}

.section-title {

  font-size: 32px;

  margin-bottom: 12px;

}

.section-subtitle {

  color: #9b9b8e;

  margin-bottom: 35px;

}

.products {

  display: grid;

  grid-template-columns: repeat(auto-fit,minmax(220px,1fr));

  gap: 25px;

}

.product {

  background: #182019;

  border: 1px solid #294b34;

  padding-bottom: 20px;

}

.product img {

  width: 100%;

  height: 260px;

  object-fit: cover;

  background: #25352a;

}

.product h3 {

  padding: 15px 15px 5px;

}

.product p {

  padding: 5px 15px;

  color: #aaa;

}

.price {

  color: #8dbb8c !important;

  font-size: 20px;

  font-weight: bold;

}

.product button {

  margin: 15px;

  padding: 12px;

  width: calc(100% - 30px);

  border: none;

  background: #315c3b;

  color: white;

  font-weight: bold;

  cursor: pointer;

}

.product button:hover {

  background: #477b50;

}

.cart {

  background: #182019;

  border: 1px solid #294b34;

  padding: 25px;

  margin-top: 35px;

}

.cart h3 {

  margin-bottom: 15px;

}

.cart-item {

  padding: 8px 0;

  border-bottom: 1px solid #344536;

}

.cart button {

  margin-top: 20px;

  padding: 14px 20px;

  background: #eee8d5;

  color: #101510;

  border: none;

  font-weight: bold;

  cursor: pointer;

}

.about {

  background: #0b0e0b;

  text-align: center;

}

.about p {

  color: #b7b7a9;

  line-height: 1.8;

  max-width: 600px;

  margin: 20px auto;

}

footer {

  padding: 30px;

  text-align: center;

  color: #888;

  background: #080b08;

}

@media(max-width:600px) {

  header {

    flex-direction: column;

    gap: 18px;

  }

  nav a {

    margin: 0 8px;

  }

  .hero {

    min-height: 360px;

  }

}

</style>

</head>

<body>

<header>

  <div class="logo">J-<span>GROOVE</span></div>

  <nav>

    <a href="#inicio">INICIO</a>

    <a href="#catalogo">TIENDA</a>

    <a href="#nosotros">NOSOTROS</a>

  </nav>

</header>

<div class="hero" id="inicio">

  <h1>J-<span>GROOVE</span></h1>

  <p>STREETWEAR · UNDERGROUND CULTURE</p>

  <a href="#catalogo">EXPLORAR COLECCIÓN</a>

</div>

<section id="catalogo">

  <h2 class="section-title">NUEVA COLECCIÓN</h2>

  <p class="section-subtitle">Vestite diferente. Marcá tu propio estilo.</p>

  <div class="products">

    <div class="product">

      <img src="https://placehold.co/600x600/183d27/eee8d5?text=J-GROOVE" alt="Remera">

      <h3>Street T-Shirt</h3>

      <p>Remera urbana</p>

      <p class="price">$ PRECIO</p>

      <button onclick="addToCart('Street T-Shirt',0)">AGREGAR AL CARRITO</button>

    </div>

    <div class="product">

      <img src="https://placehold.co/600x600/183d27/eee8d5?text=J-GROOVE" alt="Buzo">

      <h3>Urban Hoodie</h3>

      <p>Buzo streetwear</p>

      <p class="price">$ PRECIO</p>

      <button onclick="addToCart('Urban Hoodie',0)">AGREGAR AL CARRITO</button>

    </div>

    <div class="product">

      <img src="https://placehold.co/600x600/183d27/eee8d5?text=J-GROOVE" alt="Pantalón">

      <h3>Street Pants</h3>

      <p>Pantalón urbano</p>

      <p class="price">$ PRECIO</p>

      <button onclick="addToCart('Street Pants',0)">AGREGAR AL CARRITO</button>

    </div>

    <div class="product">

      <img src="https://placehold.co/600x600/183d27/eee8d5?text=J-GROOVE" alt="Accesorios">

      <h3>Urban Accessories</h3>

      <p>Accesorios streetwear</p>

      <p class="price">$ PRECIO</p>

      <button onclick="addToCart('Urban Accessories',0)">AGREGAR AL CARRITO</button>

    </div>

  </div>

  <div class="cart">

    <h3>MI CARRITO</h3>

    <div id="cart-items">Todavía no agregaste productos.</div>

    <h3 id="total">Total: $0</h3>

    <button onclick="sendWhatsApp()">FINALIZAR POR WHATSAPP</button>

  </div>

</section>

<section class="about" id="nosotros">

  <h2 class="section-title">ABOUT J-GROOVE</h2>

  <p>

    No seguimos tendencias. Creamos nuestro propio movimiento.

    Inspirados en la cultura urbana, el hip-hop y el streetwear.

    J-GROOVE representa una forma distinta de vestir y expresarse.

  </p>

</section>

<footer>

  <h3>J-GROOVE</h3>

  <p>STREETWEAR · VILLA MARÍA, CÓRDOBA</p>

  <p>© 2026 J-GROOVE. ALL RIGHTS RESERVED.</p>

</footer>

<script>

let cart = [];

function addToCart(name, price) {

  cart.push({name, price});

  updateCart();

}

function updateCart() {

  const container = document.getElementById('cart-items');

  const total = document.getElementById('total');

  container.innerHTML = '';

  if (cart.length === 0) {

    container.innerHTML = 'Todavía no agregaste productos.';

  }

  let sum = 0;

  cart.forEach((item, index) => {

    sum += item.price;

    container.innerHTML += `

      <div class="cart-item">

        ${item.name} - $${item.price}

        <button onclick="removeItem(${index})">X</button>

      </div>

    `;

  });

  total.innerText = 'Total: $' + sum;

}

function removeItem(index) {

  cart.splice(index, 1);

  updateCart();

}

function sendWhatsApp() {

  if (cart.length === 0) {

    alert('Primero agregá un producto al carrito.');

    return;

  }

  let message = 'Hola J-GROOVE! Quiero consultar por:%0A';

  cart.forEach(item => {

    message += '- ' + item.name + ' ($' + item.price + ')%0A';

  });

  message += '%0ATotal: $' +

    cart.reduce((sum,item) => sum + item.price,0);

  window.open('https://wa.me/549XXXXXXXXXX?text=' + message, '_blank');

}

</script>

</body>

</html>
