# Exercício Somando numeros

O objetivo do exercício foi realizar a soma de dois valores digitados pelo usuario.

foi utlizado:

- 2 Input type number: para cada valor colocado
- Input type button: para mandar realizar a soma entre os valores
- Function (Função) vinculada ao input Button, para realizar a operação matematica entre os valores.

A continuação o resultado:

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Somando numeros</title>
    <style>
        body {
            font: 18pt arial;
        }
        input{
            font: normal 18pt arial;
            width: 100px;
        }
        div#res {
            margin-top: 20px;
        }
    </style>
</head>
<body>
   <h1>Somando valores</h1>
    <input type="number" name="txtn1" id="txtn1"> +
    <input type="number" name="txtn2" id="txtn2">
    <input type="button" value="somar" onclick="somar()">

    <div id="res">Resultado</div>
    <script>
        function somar() {
            var tn1 = document.getElementById('txtn1')
            var tn2 = document.querySelector('input#txtn2')
            var res = document.getElementById('res')
            var n1 = Number(tn1.value)
            var n2 = Number(tn2.value)
            var s = n1 + n2
            res.innerHTML= `A soma entre ${n1} e ${n2} è igual a <strong>${s}</strong>`
            }
    </script>
</body>
</html>