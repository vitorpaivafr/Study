<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apresentação</title>

    <style>

        body {
            display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #430582;
    background-image: url("https://media.licdn.com/dms/image/v2/D4E0BAQGU6SWfxk1fDQ/company-logo_200_200/company-logo_200_200/0/1681133054218?e=2147483647&v=beta&t=V3Kcx2qywc_RoFDk54meawrqO16K8WJAfu1wY5b1ZnY");
    background-size: 100px 100px;
    background-repeat: no-repeat;
    background-position: top left;
    margin: 0;
    font-family: Arial, sans-serif;
        }

        .card {
            width: 350px;
            background: rgb(255, 255, 255);
            padding: 20px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            border-radius: 12px;
            text-align: center;
            transition: transform 0.3s ease-in-out;
        }

        .card:hover {
            transform: scale(1.05);
        }

        .icon {
            font-size: 50px;
            color: #007bff;
        }

        .eu {
            display: none;
        }

        .btn {
            margin-top: 15px;
            padding: 10px;
            width: 100%;
            border: none;
            background: blue;
            color: white;
            font-size: 16px;
            cursor: pointer;
            border-radius: 5px;
            transition: background 0.3s;
        }

        .btn:hover {
            background: #430582;
        }
    </style>
</head>
<body>


    <div class="card">
        <div class="icon">🧔🏻</div>
        <h2>Vitor Paiva</h2>
        <p>Desenvolvedor | Estudante de JavaScript</p>
        <p id="eu" class="eu">
            Sou alguém apaixonado pelo desenvolvimento, me desafio a aprender sempre e 
            sempre aprendo rapidamente com muita insistência pois sei o que quero realizar.
            Aprender e colocar em ação meu aprendizado, vai ser de fato uma realização e cada 
            código é um passo a mais para meu futuro.
        </p>
        <button id="toggleBtn" class="btn">Sobre Mim</button>
    </div>


    <script>
        const toggleBtn = document.getElementById("toggleBtn");
        const extraInfo = document.getElementById("eu");

        toggleBtn.addEventListener("click", () => {
            if (extraInfo.classList.contains("eu")) {
                extraInfo.classList.remove("eu");
                toggleBtn.textContent = "Ocultar";
            } else {
                extraInfo.classList.add("eu");
                toggleBtn.textContent = "Sobre Mim";
            }
        });
    </script>

</body>
</html>
