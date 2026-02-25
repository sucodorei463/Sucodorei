<!DOCTYPE html>  
<html lang="pt-br">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>Suco do Rei</title>  
  
<link rel="icon" type="image/jpg" href="logo.jpg">  
  
<style>  
body {  
    margin: 0;  
    font-family: Arial, sans-serif;  
    background-color: #fff8e1;  
}  
  
header {  
    background: linear-gradient(90deg, #ff9800, #ff5722);  
    color: white;  
    padding: 20px;  
    text-align: center;  
}  
  
.logo {  
    width: 200px;  
    margin-bottom: 10px;  
}  
  
nav {  
    background-color: #ff7043;  
    display: flex;  
    justify-content: center;  
    gap: 30px;  
    padding: 15px;  
}  
  
nav a {  
    color: white;  
    text-decoration: none;  
    font-weight: bold;  
}  
  
.banner {  
    background-image: url('https://images.unsplash.com/photo-1570197788417-0e82375c9371');  
    background-size: cover;  
    background-position: center;  
    height: 350px;  
    display: flex;  
    align-items: center;  
    justify-content: center;  
    color: white;  
    font-size: 38px;  
    font-weight: bold;  
    text-shadow: 2px 2px 6px black;  
}  
  
.container {  
    padding: 40px;  
    text-align: center;  
}  
  
.produtos {  
    display: grid;  
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));  
    gap: 25px;  
    margin-top: 30px;  
}  
  
.card {  
    background-color: white;  
    padding: 20px;  
    border-radius: 12px;  
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);  
}  
  
.card img {  
    width: 100%;  
    border-radius: 10px;  
    height: 180px;  
    object-fit: cover;  
}  
  
.card h3 {  
    color: #ff5722;  
}  
  
.preco {  
    font-weight: bold;  
    margin: 10px 0;  
}  
  
button {  
    background-color: #ff9800;  
    border: none;  
    padding: 10px 20px;  
    color: white;  
    border-radius: 5px;  
    cursor: pointer;  
}  
  
button:hover {  
    background-color: #e65100;  
}  
  
footer {  
    background-color: #ff5722;  
    color: white;  
    text-align: center;  
    padding: 15px;  
    margin-top: 40px;  
}  
  
/* Botão WhatsApp */  
.whatsapp-float {  
    position: fixed;  
    width: 60px;  
    height: 60px;  
    bottom: 20px;  
    right: 20px;  
    background-color: #25d366;  
    border-radius: 50%;  
    display: flex;  
    justify-content: center;  
    align-items: center;  
    box-shadow: 2px 2px 10px rgba(0,0,0,0.3);  
    z-index: 100;  
}  
  
.whatsapp-float img {  
    width: 35px;  
}  
</style>  
</head>  
  
<body>  
  
<header>  
    <img src="logo.jpg" alt="Logo Suco do Rei" class="logo">  
    <h1>Suco do Rei</h1>  
    <p>O sabor digno da realeza!</p>  
</header>  
  
<nav>  
    <a href="#produtos">Cardápio</a>  
    <a href="#contato">Contato</a>  
</nav>  
  
<div class="banner">  
    Sucos Naturais em Garrafinhas PET 🍊👑  
</div>  
  
<section class="container" id="produtos">  
    <h2>Nosso Cardápio</h2>  
    <div class="produtos">  
  
        <div class="card">  
            <img src="https://images.unsplash.com/photo-1600271886742-f049cd451bba" alt="Suco de Laranja">  
            <h3>🍊 Suco de Laranja</h3>  
            <p class="preco">500ml - R$12,00<br>300ml - R$8,00</p>  
            <button onclick="pedido('Suco de Laranja')">Pedir</button>  
        </div>  
  
        <div class="card">  
            <img src="https://images.unsplash.com/photo-1627308595181-48a3b9c1c77f" alt="Lara Mora">  
            <h3>🍊🍓 Laranja com Morango (LARA-MORA)</h3>  
            <p class="preco">500ml - R$12,00<br>300ml - R$8,00</p>  
            <button onclick="pedido('Lara Mora')">Pedir</button>  
        </div>  
  
        <div class="card">  
            <img src="https://images.unsplash.com/photo-1589308078054-8326b7e5d9b3" alt="Suco de Maracujá">  
            <h3>🥭 Suco de Maracujá</h3>  
            <p class="preco">500ml - R$12,00<br>300ml - R$8,00</p>  
            <button onclick="pedido('Suco de Maracujá')">Pedir</button>  
        </div>  
  
        <div class="card">  
            <img src="https://images.unsplash.com/photo-1567306226416-28f0efdc88ce" alt="Salada de Frutas">  
            <h3>🍍🍓 Salada de Frutas</h3>  
            <p class="preco">R$13,50</p>  
            <button onclick="pedido('Salada de Frutas')">Pedir</button>  
        </div>  
  
    </div>  
</section>  
  
<section class="container" id="contato">  
    <h2>Contato</h2>  
    <p>📍 Centro - RJ</p>  
    <p>📞 WhatsApp: (21) 99726-6412</p>  
    <p>📸 Instagram: @sucodorei__</p>  
</section>  
  
<footer>  
    © 2026 Suco do Rei - Todos os direitos reservados  
</footer>  
  
<!-- Botão flutuante WhatsApp -->  
<a href="https://wa.me/5521997266412" class="whatsapp-float" target="_blank">  
    <img src="https://cdn-icons-png.flaticon.com/512/733/733585.png" alt="WhatsApp">  
</a>  
  
<script>  
function pedido(produto) {  
    const numero = "5521997266412";  
    const mensagem = `Olá! Quero pedir: ${produto}`;  
    const url = `https://wa.me/${numero}?text=${encodeURIComponent(mensagem)}`;  
    window.open(url, '_blank');  
}  
</script>  
  
</body>  
</html>  
