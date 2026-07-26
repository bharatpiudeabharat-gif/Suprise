<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Surprise</title>

<style>
body{
margin:0;
background:black;
display:flex;
justify-content:center;
align-items:center;
height:100vh;
font-family:sans-serif;
overflow:hidden;
}

#lock{
text-align:center;
color:white;
}

input{
padding:12px;
border:none;
border-radius:8px;
font-size:18px;
text-align:center;
}

button{
padding:12px 20px;
margin-top:10px;
border:none;
border-radius:8px;
background:#ff4d6d;
color:white;
font-size:18px;
}

#content{
display:none;
text-align:center;
color:white;
}

img{
width:280px;
border-radius:15px;
margin:10px;
}

h1{
color:#ff8fab;
}
</style>
</head>

<body>

<div id="lock">
<h2>🔒 Open the Surprise</h2>
<p>Enter the secret word</p>

<input type="password" id="pass" placeholder="Password">
<br>
<button onclick="check()">Open ❤️</button>
</div>

<div id="content">
<h1>❤️ For You ❤️</h1>

<img src="photo1.jpg">
<img src="photo2.jpg">

<audio controls autoplay loop>
<source src="song.mp3" type="audio/mpeg">
</audio>

</div>

<script>
function check(){
if(document.getElementById("pass").value=="aashal"){
document.getElementById("lock").style.display="none";
document.getElementById("content").style.display="block";
}else{
alert("Wrong Password ❤️");
}
}
</script>

</body>
</html>
