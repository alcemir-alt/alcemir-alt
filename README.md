<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portal de Notícias Completo</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #333;
            color: white;
            padding: 20px;
            text-align: center;
        }
        nav {
            background-color: #444;
            color: white;
            display: flex;
            justify-content: space-around;
            padding: 15px;
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 5px 10px;
        }
        nav a:hover {
            background-color: #555;
        }
        .content {
            display: flex;
            flex-wrap: wrap;
            padding: 20px;
        }
        .main-content {
            flex: 70%;
            padding: 20px;
        }
        .sidebar {
            flex: 30%;
            padding: 20px;
            background-color: #eee;
        }
        article {
            background-color: white;
            margin-bottom: 20px;
            padding: 15px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        article img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
        }
        footer {
            background-color: #333;
            color: white;
            padding: 20px;
            text-align: center;
        }
        .search-bar {
            padding: 10px;
            text-align: center;
        }
        .search-bar input {
            padding: 10px;
            width: 80%;
            font-size: 16px;
        }
        .search-bar button {
            padding: 10px;
            font-size: 16px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Portal de Notícias</h1>
    </header>
    <nav>
        <a href="#">Início</a>
        <a href="#">Política</a>
        <a href="#">Esportes</a>
        <a href="#">Entretenimento</a>
        <a href="#">Economia</a>
        <a href="#">Contato</a>
    </nav>
    <div class="search-bar">
        <input type="text" placeholder="Buscar notícias...">
        <button>Buscar</button>
    </div>
    <div class="content">
        <div class="main-content">
            <article>
                <h2>Título da Notícia 1</h2>
                <img src="imagem1.jpg" alt="Imagem da Notícia 1">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vehicula diam in urna facilisis, in efficitur velit posuere.</p>
            </article>
            <article>
                <h2>Título da Notícia 2</h2>
                <img src="imagem2.jpg" alt="Imagem da Notícia 2">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vehicula diam in urna facilisis, in efficitur velit posuere.</p>
            </article>
            <article>
                <h2>Título da Notícia 3</h2>
                <img src="imagem3.jpg" alt="Imagem da Notícia 3">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent vehicula diam in urna facilisis, in efficitur velit posuere.</p>
            </article>
        </div>
        <div class="sidebar">
            <h3>Últimas Notícias</h3>
            <ul>
                <li><a href="#">Notícia recente 1</a></li>
                <li><a href="#">Notícia recente 2</a></li>
                <li><a href="#">Notícia recente 3</a></li>
                <li><a href="#">Notícia recente 4</a></li>
            </ul>
            <h3>Categorias</h3>
            <ul>
                <li><a href="#">Política</a></li>
                <li><a href="#">Esportes</a></li>
                <li><a href="#">Entretenimento</a></li>
                <li><a href="#">Economia</a></li>
            </ul>
        </div>
    </div>
    <footer>
        <p>&copy; 2025 Portal de Notícias. Todos os direitos reservados.</p>
    </footer>
    <script>
        // JavaScript para funcionalidades interativas
        document.querySelectorAll('nav a').forEach(link => {
            link.addEventListener('mouseover', () => {
                link.style.backgroundColor = '#666';
            });
            link.addEventListener('mouseout', () => {
                link.style.backgroundColor = '';
            });
        });

        const searchBar = document.querySelector('.search-bar input');
        const searchButton = document.querySelector('.search-bar button');
        searchButton.addEventListener('click', () => {
            alert(`Buscando por: ${searchBar.value}`);
        });
    </script>
</body>
</html>
