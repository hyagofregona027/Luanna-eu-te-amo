# Luanna-eu-te-amo
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Hyago ❤️ Luanna</title>

<style>

body{
margin:0;
font-family:Arial, sans-serif;
background:linear-gradient(135deg,#ff758c,#ff7eb3);
color:white;
text-align:center;
overflow-x:hidden;
}

.container{
padding:40px;
max-width:900px;
margin:auto;
}

h1{
font-size:50px;
}

.timeline{
margin-top:30px;
font-size:20px;
}

.bigcounter{
margin-top:40px;
font-size:40px;
font-weight:bold;
background:rgba(255,255,255,0.1);
padding:20px;
border-radius:20px;
}

.gallery{
margin-top:40px;
display:grid;
grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
gap:15px;
}

.gallery img{
width:100%;
border-radius:15px;
box-shadow:0 10px 20px rgba(0,0,0,0.4);
}

button{
margin-top:40px;
padding:15px 30px;
font-size:20px;
border:none;
border-radius:30px;
background:white;
color:#ff4d6d;
cursor:pointer;
font-weight:bold;
}

button:hover{
transform:scale(1.05);
}

#mensagem{
display:none;
margin-top:30px;
font-size:22px;
max-width:600px;
margin-left:auto;
margin-right:auto;
}

.flower{
position:fixed;
top:-10px;
font-size:20px;
animation:fall linear forwards;
}

@keyframes fall{
to{
transform:translateY(110vh);
}
}

</style>
</head>

<body>

<div class="container">

<h1>Hyago ❤️ Luanna</h1>

<p>Desde que você entrou na minha vida tudo ficou mais bonito.</p>

<div class="timeline">
<p>✨ 14/06/2025 — O dia em que nos conhecemos</p>
<p>🥰 20/06/2025 — Nosso primeiro encontro</p>
<p>🏆 21/06/2025 — Você foi no meu campeonato e depois saímos</p>
<p>💍 07/09/2025 — O dia que começamos a namorar</p>
</div>

<div class="bigcounter">

<p>❤️ Nosso namoro:</p>
<p id="contador"></p>

</div>

<h2>Nossa música 🎵</h2>

<iframe style="border-radius:12px"
src="https://open.spotify.com/embed/track/2WwNvrW6o7z3N6yipgre6R"
width="100%"
height="152"
frameBorder="0"
allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture">
</iframe>

<h2>Nossos Momentos 📸</h2>

<div class="gallery">
<img src="foto1.jpg">
<img src="foto2.jpg">
<img src="foto3.jpg">
<img src="foto4.jpg">
</div>

<button onclick="mostrarMensagem()">Clique aqui Luanna ❤️</button>

<div id="mensagem">
<p>
Luanna,

desde o dia que te conheci minha vida mudou completamente.
Cada momento com você é especial e eu sou muito feliz por ter você comigo.

Obrigado por cada sorriso, cada abraço e cada momento que vivemos.

Eu te amo ❤️
</p>
</div>

</div>

<script>

function atualizarContador(){

const inicio = new Date("2025-09-07");
const agora = new Date();

let diff = agora - inicio;

let segundos = Math.floor(diff/1000)%60;
let minutos = Math.floor(diff/60000)%60;
let horas = Math.floor(diff/3600000)%24;
let dias = Math.floor(diff/86400000);

document.getElementById("contador").innerHTML =
dias+" dias "+horas+"h "+minutos+"m "+segundos+"s";

}

setInterval(atualizarContador,1000);

function mostrarMensagem(){
document.getElementById("mensagem").style.display="block";
}

function criarFlor(){

const flor=document.createElement("div");

flor.classList.add("flower");

flor.innerHTML="🌸";

flor.style.left=Math.random()*100+"vw";
flor.style.animationDuration=(Math.random()*4+3)+"s";

document.body.appendChild(flor);

setTimeout(()=>{
flor.remove();
},7000);

}

setInterval(criarFlor,400);

</script>

</body>
</html>
