# Exercício de eventos com imagem

O objetivo deste exercício foi criar 3 interações com a imagem criada a partir de eventos. Nesse exercício foram utilizados os eventos:

- click
- mouseenter
- mouseout

Para cada interação a partir dos eventos desginados, foi criado uma função.

A continuação o resultado: 

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eventos DOM</title>
    <style>
        div#area {
           background: rgb(63, 177, 63); 
           font: normal 20pt arial;
            color: white;
            height: 200px;
            width: 200px;
            line-height: 200px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div id="area"><!--Si quiero cambiar los evento en html, colocar: onclick="clicar()" onmouseenter="entrar()" onmouseout="sair()"-->
        interaja...
    </div>
    <script>
        var a = document.getElementById('area') //getElementById a la variable a se modifica por el ID al div "area"
        a.addEventListener("click", clicar)
        a.addEventListener("mouseenter", entrar)
        a.addEventListener("mouseout", sair)
​        function clicar(){
​            a.innerText = 'Clicou!'
​            a.style.background= "red"
​        }
​        function entrar(){
​            a.innerText='Entrou!'
​        }
​        function sair(){
​            a.innerText='Saiu!'
​            a.style.background='rgb(63, 177, 63)'
​        }
​    </script>
</body>
</html>

