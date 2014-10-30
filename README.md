Javascript qui affiche une phrase aléatoire
<pwd>    <span id='phrase'>Ici la phrase</span><br> </pwd>


Avec un bouton en dessous qui affiche une nouvelle phrase aléatoire à la place :
    <button onclick='nouvelle_phrase()'>Changer la phrase</button>

Les phrases sont issues d'un fichier texte (files.js)

<html>
<head>
    <script type="text/javascript" src='files.js'></script>
</head>
  
<body>
    <span id='phrase'>ici  ta phrase</span><br>
    <button onclick='nouvelle_phrase()'>Nouvelle phrase</button>
  
<script>
function nouvelle_phrase(){
    var nb = Math.floor(Math.random() * files.length);
    document.getElementById('phrase').innerHTML=files[nb];
}
nouvelle_phrase();    
 
</script>
  
</body>
</html>
