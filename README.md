<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mirzoxid.Bek</title>

<style>
*{
margin:02к3;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:#0f0f0f;
color:white;
display:flex;
justify-content:center;
align-items:center;
min-height:100vh;
padding:20px;
}

.container{
width:100%;
max-width:420px;
background:#1b1b1b;
padding:25px;
border-radius:18px;
box-shadow:0 0 20px rgba(0,255,255,.25);
}

h1{
text-align:center;
color:#00e5ff;
margin-bottom:10px;
}

p{
text-align:center;
color:#bbb;
margin-bottom:20px;
}

input,select,textarea{
width:100%;
padding:14px;
margin:8px 0;
border:none;
border-radius:10px;
background:#2b2b2b;
color:white;
font-size:16px;
}

textarea{
height:100px;
resize:none;
}

button{
width:100%;
padding:15px;
border:none;
border-radius:10px;
background:#00c853;
color:white;
font-size:18px;
font-weight:bold;
cursor:pointer;
margin-top:10px;
}

button:hover{
background:#00a844;
}

#msg{
text-align:center;
margin-top:15px;
color:#00ff99;
font-weight:bold;
}
</style>
</head>

<body>

<div class="container">

<h1>Mirzoxid.Bek</h1>
<p>Buyurtma qoldiring</p>

<input type="text" id="name" placeholder="Ismingiz">

<input type="tel" id="phone" placeholder="+998 XX XXX XX XX">

<select id="service">
<option>Video montaj</option>
<option>Reklama roligi</option>
<option>SMM</option>
<option>Mobil videografiya</option>
<option>Boshqa</option>
</select>

<textarea id="comment" placeholder="Buyurtma haqida yozing..."></textarea>

<button onclick="sendOrder()">Buyurtma yuborish</button>

<div id="msg"></div>

</div>

<script>
function sendOrder(){

let name=document.getElementById("name").value;
let phone=document.getElementById("phone").value;
let service=document.getElementById("service").value;

if(name=="" || phone==""){
document.getElementById("msg").innerHTML="❌ Ism va telefonni kiriting!";
return;
}

document.getElementById("msg").innerHTML="✅ Buyurtmangiz qabul qilindi! Tez orada siz bilan bog'lanamiz.";

}
</script>

</body>
</html>
