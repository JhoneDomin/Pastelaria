# Pastelaria<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Pastelaria do Antonio</title>

<style>

body{
font-family: Arial;
background:#fff7e6;
text-align:center;
margin:0;
}

header{
background:#ff9800;
color:white;
padding:20px;
font-size:28px;
font-weight:bold;
}

.produtos{
display:flex;
flex-wrap:wrap;
justify-content:center;
gap:20px;
padding:30px;
}

.card{
background:white;
width:220px;
padding:20px;
border-radius:12px;
box-shadow:0 4px 10px rgba(0,0,0,0.1);
}

.card h3{
margin:10px 0;
}

.preco{
color:#ff5722;
font-size:18px;
font-weight:bold;
}

button{
background:#25D366;
color:white;
border:none;
padding:12px;
border-radius:8px;
cursor:pointer;
margin-top:10px;
width:100%;
font-size:16px;
}

button:hover{
background:#1ebe5d;
}

</style>
</head>

<body>

<header>
🥟 Pastelaria do Antonio
</header>

<h2>Escolha seu pastel</h2>

<div class="produtos">

<div class="card">
<h3>Pastel de Carne</h3>
<p class="preco">R$ 8,00</p>
<button onclick="pedir('Pastel de Carne')">Pedir no WhatsApp</button>
</div>

<div class="card">
<h3>Pastel de Queijo</h3>
<p class="preco">R$ 7,00</p>
<button onclick="pedir('Pastel de Queijo')">Pedir no WhatsApp</button>
</div>

<div class="card">
<h3>Pastel de Frango</h3>
<p class="preco">R$ 8,00</p>
<button onclick="pedir('Pastel de Frango')">Pedir no WhatsApp</button>
</div>

<div class="card">
<h3>Pastel de Pizza</h3>
<p class="preco">R$ 9,00</p>
<button onclick="pedir('Pastel de Pizza')">Pedir no WhatsApp</button>
</div>

<div class="card">
<h3>Pastel de Calabresa</h3>
<p class="preco">R$ 8,50</p>
<button onclick="pedir('Pastel de Calabresa')">Pedir no WhatsApp</button>
</div>

</div>

<script>

function pedir(produto){

let numero = "5585991923386"

let mensagem = "Olá, quero pedir um " + produto

let url = "https://wa.me/" + numero + "?text=" + encodeURIComponent(mensagem)

window.open(url)

}

</script>

</body>
</html>
