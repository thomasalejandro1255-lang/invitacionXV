<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>15 Años María Camila</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family: "Georgia", serif;
}

body{
    background:#071a40;
    background-image:
    radial-gradient(circle at top, #153d87 0%, #071a40 60%);
    color:#f4d78a;
    min-height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    padding:30px;
}

.container{
    max-width:900px;
    width:100%;
    background:rgba(0,0,0,.25);
    border:2px solid #d4af37;
    border-radius:30px;
    padding:40px;
    text-align:center;
    box-shadow:0 0 30px rgba(212,175,55,.3);
}

h1{
    font-size:70px;
    color:#f4d78a;
    margin-bottom:10px;
}

h2{
    font-size:26px;
    margin-bottom:25px;
    letter-spacing:3px;
}

.descripcion{
    font-size:20px;
    margin-bottom:30px;
    line-height:1.6;
    color:#fff;
}

.info{
    margin:25px 0;
    font-size:22px;
}

.linea{
    width:120px;
    height:2px;
    background:#d4af37;
    margin:20px auto;
}

.bloque{
    margin-top:30px;
}

input{
    width:100%;
    max-width:420px;
    padding:15px;
    border-radius:12px;
    border:2px solid #d4af37;
    outline:none;
    font-size:16px;
    text-align:center;
    margin-bottom:20px;
}

.botones{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:15px;
}

.btn{
    display:inline-block;
    padding:16px 26px;
    text-decoration:none;
    color:#f4d78a;
    border:2px solid #d4af37;
    border-radius:15px;
    background:#0c2f73;
    font-weight:bold;
    transition:.3s;
    cursor:pointer;
}

.btn:hover{
    transform:translateY(-3px);
    background:#17479f;
}

.btn-full{
    width:100%;
    max-width:500px;
}

.footer{
    margin-top:40px;
    font-size:34px;
    font-style:italic;
}

@media(max-width:768px){

    h1{
        font-size:50px;
    }

    .botones{
        flex-direction:column;
    }

    .btn{
        width:100%;
    }
}

</style>
</head>

<body>

<div class="container">

    <h2>ESTÁS INVITADO A LOS</h2>

    <h1>15 Años</h1>

    <h2>María Camila</h2>

    <p class="descripcion">
        Hay momentos en la vida que se vuelven inolvidables cuando los compartimos
        con las personas que amamos.<br>
        Por eso quiero invitarte a celebrar conmigo este día tan especial.
    </p>

    <div class="linea"></div>

    <div class="info">
        📅 19 de diciembre de 2026
    </div>

    <div class="info">
        🕗 8:00 p.m.
    </div>

    <div class="info">
        📍 Xilón Club Palmira
    </div>

    <div class="linea"></div>

    <div class="botones">

        https://maps.app.goo.gl/5Xab6T8yonCxsey48
           📍 VER UBICACIÓN
        </a>

        https://wa.me/573005773159?text=Hola,%20confirmo%20mi%20asistencia%20a%20los%2015%20años%20de%20María%20Camila.
           💬 CONFIRMAR ASISTENCIA
        </a>

    </div>

    <div class="bloque">

        <h2>CONFIRMAR ACOMPAÑANTE</h2>

        <input
            type="text"
            id="acompanante"
            placeholder="Escriba aquí el nombre del acompañante">

        <br>

        <button
            class="btn"
            onclick="enviarAcompanante()">
            👥 ENVIAR ACOMPAÑANTE
        </button>

    </div>

    <div class="bloque">

        evento.ics
        📅 AGREGAR AL CALENDARIO
        </a>

    </div>

    <div class="footer">
        ¡Te espero!
    </div>

</div>

<script>

function enviarAcompanante(){

    let nombre =
    document.getElementById('acompanante').value.trim();

    if(nombre === ""){
        alert("Por favor escribe el nombre del acompañante.");
        return;
    }

    let mensaje =
    "Hola, mi acompañante para los 15 años de María Camila es: " + nombre;

    window.open(
        "https://wa.me/573005773159?text=" +
        encodeURIComponent(mensaje),
        "_blank"
    );
}

</script>

</body>
</html>

