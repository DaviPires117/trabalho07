<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Receita de Bolo de Chocolate</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Receita de Bolo de Chocolate</h1>
    </header>
    <section class="content">
        <div class="ingredientes">
            <h2>Ingredientes:</h2>
            <ul>
                <li>2 xícaras de farinha de trigo</li>
                <li>1 xícara de cacau em pó</li>
                <li class="destaque">1 xícara de açúcar</li>
                <li>1 colher de chá de fermento em pó</li>
                <li>1/2 colher de chá de sal</li>
            </ul>
        </div>
        <div class="instrucoes">
            <h2>Modo de Preparo:</h2>
            <ol>
                <li class="passo" data-passo="1">Pré-aqueça o forno a 180°C.</li>
                <li class="passo" data-passo="2">Em uma tigela, misture a farinha, o cacau em pó, o açúcar, o fermento e o sal.</li>
                <li class="passo" data-passo="3">Adicione os ingredientes líquidos e misture até obter uma massa homogênea.</li>
                <li class="passo" data-passo="4">Despeje a massa em uma forma untada e enfarinhada.</li>
                <li class="passo" data-passo="5">Asse no forno por 30-35 minutos.</li>
                <li class="passo" data-passo="6">Deixe esfriar antes de servir.</li>
            </ol>
        </div>
    </section>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    text-align: center;
    background-color: #3399FF;
    color: #fff;
    padding: 20px 0;
}

.content {
    display: flex;
    justify-content: space-between;
    margin: 20px;
}

.ingredientes, .instrucoes {
    flex-basis: calc(50% - 20px);
    padding: 10px;
    border: 1px solid #ccc;
}

ul, ol {
    list-style: none;
    padding: 0;
}

li::before {
    content: '• ';
    color: #FF5733;
}

.destaque {
    font-weight: bold;
}

.passo::before {
    content: attr(data-passo) '. ';
    color: #3399FF;
}

.passo:nth-child(even) {
    background-color: #F2F2F2;
}

.passo:nth-child(odd) {
    background-color: #E5E5E5;
}
