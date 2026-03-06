<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Hyago ❤️ Luanna</title>

<style>

body{
margin:0;
font-family: 'Segoe UI', sans-serif;
background:linear-gradient(160deg,#ff7aa2,#ffb6c1);
color:white;
text-align:center;
overflow-x:hidden;
}

section{
padding:80px 20px;
opacity:0;
transform:translateY(30px);
transition:1s;
}

section.show{
opacity:1;
transform:translateY(0);
}

h1{
font-size:60px;
margin-bottom:10px;
}

.subtitle{
font-size:22px;
opacity:0.9;
}

.counter{
font-size:45px;
font-weight:bold;
margin-top:30px;
}

.gallery{
display:flex;
flex-direction:column;
gap:40px;
align-items:center;
}

.gallery img{
width:80%;
max-width:500px;
border-radius:20px;
box-shadow:0 20px 40px rgba(0,0,0,0.4);
transition:0.6s;
}

.gallery img:hover{
transform:scale(1.05);
}

button{
margin-top:40px;
padding:18px 40px;
font-size:22px;
border:none;
border-radius:40px;
background:white;
color:#ff4d7a;
font-weight:bold;
cursor:pointer;
}

button:hover{
transform:scale(1.05);
}

#mensagem{
display:none;
max-width:600px;
margin:auto;
margin-top:40px;
font-size:22px;
line-height:1.6;
}

.flower{
position:fixed;
top:-20px;
font-size:20px;
animation:fall linear forwards;
}

@keyframes fall{
to{
transform:translateY(110vh);
}
}

iframe{
margin-top:40px;
border-radius:15px;
}

</style>
</head>

<body>

<section>
<h1>Hyago ❤️ Luanna</h1>
<p class="subtitle">Nossa história começou em 14 de junho de 2025</p>
</section>

<section>

<h2>Estamos juntos há</h2>

<div class="counter" id="contador"></div>

</section>

<section class="gallery">

<img src="foto1.jpg">
<img src="foto2.jpg">
<img src="foto3.jpg">

</section>

<section>

<h2>Nossa música 🎵</h2>

<iframe
src="https://open.spotify.com/embed/track/2WwNvrW6o7z3N6yipgre6R"
width="80%"
height="152"
frameborder="0"
allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture">
</iframe>

</section>

<section>

<button onclick="mostrarMensagem()">Clique aqui Luanna ❤️</button>

<div id="mensagem">
Luanna,

desde o dia que te conheci minha vida ficou muito mais bonita.

Cada momento com você é especial, e eu agradeço todos os dias por ter você comigo.

Obrigado por fazer parte da minha vida.

Eu te amo ❤️
</div>

</section>

<script>

function atualizarContador(){

const inicio = new Date("2025-09-07");
const agora = new Date();

let diff = agora - inicio;

let dias = Math.floor(diff / (1000*60*60*24));
let horas = Math.floor(diff / (1000*60*60)) % 24;
let minutos = Math.floor(diff / (1000*60)) % 60;
let segundos = Math.floor(diff / 1000) % 60;

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

flor.style.animationDuration=(Math.random()*5+4)+"s";

document.body.appendChild(flor);

setTimeout(()=>{
flor.remove();
},8000);

}

setInterval(criarFlor,500);

const sections=document.querySelectorAll("section");

window.addEventListener("scroll",()=>{

sections.forEach(sec=>{

const top=sec.getBoundingClientRect().top;

if(top<window.innerHeight-100){
sec.classList.add("show");
}

});

});

</script>

</body>
</html>
