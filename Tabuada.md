# Repository-CRISTIAN
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> TABUADA </title>
   
    <style>

body { font: 12pt Arial; }
h1, h2, h3 { font-family: 'Pacifico', cursive; font-weight: normal;}
input[type=number] { font-size: 12pt; }
input[type=submit] { 
    background-color: rgb(97, 109, 177); 
    color: white; 
    font-size: 12pt; 
    padding: 5px; 
}
    </style>
    
</head>
<body>
    <h1>SUPER TABUADA</h1>
    <p>Digite um número na caixa a seguir e te mostrarei a tabuada dele.</p>
    <section id="entrada">
        <form action="#" method="get">
            <p>
                <label for="fn1">Número: </label>
                <input type="number" name="num" id="fnum" placeholder="Numero: ">
                <input  type="submit" value="Tabuada" formaction="javascript:tabuada()">
            </p>
        
        </form>
    </section>
    <section id="saida">
        <p>Preencha os dados acima e aperte o botão.</p>
    </section>

 <script>

function tabuada() {
    var saida = document.getElementById('saida')
    var n = Number(document.getElementById('fnum').value)

    saida.innerHTML = `<h2>Tabuada de ${n}</h2>`
    var  c = 1
    while (c <= 10) {
        saida.innerHTML += `${n} x ${c} = <strong>${n * c}</strong><br>`
        c ++
    }
} 

    </script>
 </body>
</html>
