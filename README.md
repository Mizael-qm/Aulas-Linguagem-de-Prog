<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <html>

    <head>
        <title>Sistema Escolar</title>
    </head>

    <style>
        body {
            background-color: rgba(223, 214, 223, 0.192)
        }

        .titulo {
            font-size: 20px;
            color: rgb(27, 25, 25);
            margin-top: 90px;
            text-align: center;

        }
        .formulario{
            background-color: aquamarine;
            width: 600px;
            padding: 20px;
            border-radius: 8px;
            border: 2px solid black;
            margin: auto;
        }
        .cadastrar{
            cursor: pointer;
            margin: auto;
            display: block;
        }
        .resultado{
            background-color: blue;
            width: 450px;
            padding: 20px;
            border-radius: 8px;
            border: 2px solid black;
            margin: auto;
            margin-top: 50px;
            display: none;


        }
    
    </style>

<body>

    <div class="titulo">
        <h1> EEB Dom Jaime de Barros Câmara</h1>
        <p>Preencha o formulário abaixo para cadastrar um novo aluno</p>

    </div>

    <div class="formulario">
    
        <form>
            <label for="nome">Nome</label>
            <input type="text" id="nome" name="nome"><br><br>

            <label for="dataNasc">Data de Nascimento</label>
            <input type="date" id= "dataNasc" name="dataNasc"><br><br>

            <label for="cpf">CPF: </label>
            <input type="text" id="cpf" name="cpf"><br><br>

            <label for="email">Email:</label>
            <input type="text" id="email" name="email"><br><br>

            <label for="cidade">Cidade:</label>
            <input type="text" id="cidade" name="cidade"><br><br>

            <label for="escola">Escola:</label>
            <input type="text" id="escola" name="escola"><br><br>

            <label for="estado natal">Estado Natal:</label>
            <input type="text" id="estado natal" name="estado natal"><br><br>

            <button type="button" class="cadastrar" onclick="mostrarDados()" >Cadastrar</button>

            


        </form>
    </div>

    <div id="resultado" class="resultado">
    </div>

    <script>
        function mostrarDados(){
            let nome = document.getElementById("nome").value;
            let dataNasc = document.getElementById("dataNasc").value;
            let cpf = document.getElementById("cpf").value;
            let email = document.getElementById("email").value;
            let cidade = document.getElementById("cidade").value;
            let escola = document.getElementById("escola").value;
            let estadonatal = document.getElementById("estado natal").value;
            

            let resultado = document.getElementById("resultado")

            document.getElementById("resultado").innerHTML = "<h2>Dados Informador: <h2>" +
                "Nome: " + nome + "<br>" +
                "Data de Nascimento: " + dataNasc + "<br>" +
                "CPF: " + cpf + "<br>" +
                "Email:" + email + "<br>" +
                "Cidade:" + cidade + "<br>" +
                "Escola:" + escola + "<br>" +
                "Estado Natal:" + estadonatal + "<br>";

                resultado.style.display ="block"

                
        }
    </script>
</body>

</html># Aulas-Linguagem-de-Prog
Códigos desenvolvidos nas aulas de linguagem de prog4ramação java.
