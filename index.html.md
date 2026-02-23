<!DOCTYPE html>  
<html lang="fr">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>Le Quotidien Express – Actualités</title>  
  
<style>  
body{  
  margin:0;  
  font-family: Georgia, serif;  
  background:#ffffff;  
  color:#111;  
}  
  
header{  
  position:sticky;  
  top:0;  
  background:white;  
  border-bottom:1px solid #ddd;  
  padding:15px;  
  display:flex;  
  justify-content:space-between;  
  align-items:center;  
  z-index:1000;  
}  
  
.logo{  
  font-size:22px;  
  font-weight:bold;  
}  
  
nav a{  
  margin:0 10px;  
  text-decoration:none;  
  color:#111;  
  font-weight:600;  
}  
  
nav a:hover{  
  text-decoration:underline;  
}  
  
.ticker{  
  background:#f5f5f5;  
  padding:8px;  
  font-size:14px;  
  overflow:hidden;  
  white-space:nowrap;  
}  
  
.ticker span{  
  display:inline-block;  
  padding-left:100%;  
  animation:scroll 20s linear infinite;  
}  
  
@keyframes scroll{  
  0%{transform:translateX(0)}  
  100%{transform:translateX(-100%)}  
}  
  
.container{  
  max-width:1000px;  
  margin:auto;  
  padding:20px;  
}  
  
.hero{  
  margin-bottom:30px;  
}  
  
.hero img{  
  width:100%;  
  border-radius:8px;  
}  
  
.hero h1{  
  font-size:32px;  
  margin-top:15px;  
}  
  
.card{  
  border-top:1px solid #ddd;  
  padding:15px 0;  
  cursor:pointer;  
}  
  
.card:hover{  
  background:#fafafa;  
}  
  
footer{  
  border-top:1px solid #ddd;  
  padding:20px;  
  text-align:center;  
  margin-top:40px;  
  font-size:14px;  
}  
  
button{  
  padding:6px 12px;  
  border:1px solid #111;  
  background:white;  
  cursor:pointer;  
}  
  
.dark{  
  background:#111;  
  color:#eee;  
}  
  
.dark header{  
  background:#111;  
  color:#eee;  
}  
  
.dark nav a{  
  color:#eee;  
}  
</style>  
</head>  
  
<body>  
  
<header>  
  <div class="logo">Le Quotidien Express</div>  
  <nav>  
    <a href="#" onclick="showHome()">Accueil</a>  
    <a href="#" onclick="showAbout()">À propos</a>  
    <a href="#" onclick="showContact()">Contact</a>  
  </nav>  
  <button onclick="toggleDark()">Mode sombre</button>  
</header>  
  
<div class="ticker">  
  <span>DERNIÈRE MINUTE • Une étude évoque un gain de 11% sur les trajets piétons • Un institut annonce une expérimentation national • Documents internes consultés</span>  
</div>  
  
<div class="container" id="content">  
  
<!-- HOME -->  
<div id="home">  
  
<div class="hero" onclick="showArticle()">  
<img src="https://images.unsplash.com/photo-1520975693411-b9f2f2ef3a3b?auto=format&fit=crop&w=1400&q=60">  
<h1>Des ‘voies rapides’ pour piétons pressés bientôt expérimentées dans plusieurs grandes villes françaises</h1>  
<p>Pour réduire les embouteillages sur les trottoirs, des municipalités testeraient des couloirs réservés aux marcheurs rapides.</p>  
</div>  
  
<h2>À lire aussi</h2>  
  
<div class="card">Des chercheurs prouvent que les devoirs rendent les élèves moins intelligents</div>  
<div class="card">La pluie artificielle testée dans le sud-ouest de la France</div>  
<div class="card">Une nouvelle loi limiterait le temps d’écran des adolescents à 2 heures par jour</div>  
<div class="card">L’océan Atlantique aurait reculé de 5 mètres en une nuit</div>  
  
</div>  
  
<!-- ARTICLE -->  
<div id="article" style="display:none">  
  
<h1>Des ‘voies rapides’ pour piétons pressés bientôt expérimentées</h1>  
<p><strong>23 février 2026 – Par Élise Garnier</strong></p>  
  
<img src="https://images.unsplash.com/photo-1520975867597-0b273a0ff7d5?auto=format&fit=crop&w=1200&q=60">  
  
<p>Dans plusieurs centres-villes, la densité piétonne atteint désormais des niveaux inédits. Selon des documents internes, des municipalités envisageraient de tester des couloirs dédiés aux marcheurs rapides.</p>  
  
<h2>Une expérimentation en centre-ville</h2>  
<p>Le dispositif serait expérimenter pendant 6 mois dans 4 villes pilotes, sur 12 zones test.</p>  
  
<h2>Réactions contrastées</h2>  
<p>“La marche est devenue un mode de transport structurant”, explique Marc Delattre, sociologue urbain.</p>  
  
<p>Laura, 29 ans, témoigne : “Quand je sors du métro, ça bouchonne. Si une voie rapide existe, je la prends.”</p>  
  
<h3>Chiffres clés</h3>  
<ul>  
<li>4 villes pilotes</li>  
<li>12 zones test</li>  
<li>6 mois d’expérimentation</li>  
<li>Budget estimé : 2,8 millions d’euros</li>  
</ul>  
  
<button onclick="showHome()">Retour à l’accueil</button>  
  
</div>  
  
<!-- ABOUT -->  
<div id="about" style="display:none">  
<h1>À propos</h1>  
<p>Ce site est un projet scolaire sur les fake news.</p>  
<p>Les articles sont inventés mais présentés comme crédibles afin d'apprendre à repérer les signes : sources floues, chiffres trop précis, détails étrange.</p>  
<button onclick="showHome()">Retour</button>  
</div>  
  
<!-- CONTACT -->  
<div id="contact" style="display:none">  
<h1>Contact</h1>  
<p>Formulaire fictif.</p>  
<input placeholder="Votre email"><br><br>  
<textarea placeholder="Votre message"></textarea><br><br>  
<button>Envoyer</button>  
<button onclick="showHome()">Retour</button>  
</div>  
  
</div>  
  
<footer>  
© 2026 Le Quotidien Express – Projet pédagogique  
</footer>  
  
<script>  
function showHome(){  
  document.getElementById("home").style.display="block";  
  document.getElementById("article").style.display="none";  
  document.getElementById("about").style.display="none";  
  document.getElementById("contact").style.display="none";  
}  
  
function showArticle(){  
  document.getElementById("home").style.display="none";  
  document.getElementById("article").style.display="block";  
}  
  
function showAbout(){  
  document.getElementById("home").style.display="none";  
  document.getElementById("about").style.display="block";  
}  
  
function showContact(){  
  document.getElementById("home").style.display="none";  
  document.getElementById("contact").style.display="block";  
}  
  
function toggleDark(){  
  document.body.classList.toggle("dark");  
}  
</script>  
  
</body>  
</html>  
