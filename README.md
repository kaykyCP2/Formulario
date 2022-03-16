# Formulario
<html>

<head>
    <meta charset="utf-8">
    <title> Formulario </title>

</head>

<body>
    <h1> Formulario </h1>
    <p id="p1"> preencha abaixo </p>

    Nome: <input id="idnome" type="text"> </input>
    <br>
    Sobrenome:<input id="idsobrenome" type="text"> </input>
    <br>
    Idade: <input id="ididade" type="number"> </input>
    <br>
    Cidade:<input id="idcidade" type="text"> </input>
    <br>
    Estado:<input id="idestado" type="text" maxlength="2"> </input>
    


    <br>
    <button onclick="preencher()"> Enviar </button>
    <p= id="idline" type="text"> </p>

    <script>
        function preencher() {
            document.getElementById("p1").innerHTML = "Formulario preenchido ";



            var nome = document.getElementById("idnome").value;
            var sobrenome = document.getElementById("idsobrenome").value;
            var Idade= document.getElementById("ididade").value;
            var cidade= document.getElementById("idcidade").value;
            var Estado= document.getElementById("idestado").value;
            var informacoes = nome + " " + sobrenome + " tem" + Idade + "anos e mora em " +  cidade + "/" + Estado;
            document.getElementById("idline").innerHTML= informacoes ;
            
        }
    </script>
