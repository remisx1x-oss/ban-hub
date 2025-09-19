<!DOCTYPE html>

<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Juegos Desbloqueados Online</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

```
    body {
        font-family: 'Arial', sans-serif;
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        min-height: 100vh;
        color: white;
    }

    .header {
        background: rgba(0, 0, 0, 0.3);
        backdrop-filter: blur(10px);
        padding: 1rem 0;
        position: sticky;
        top: 0;
        z-index: 100;
        box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
    }

    .nav-container {
        max-width: 1200px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 2rem;
    }

    .logo {
        font-size: 2rem;
        font-weight: bold;
        background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
        background-clip: text;
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        animation: glow 2s ease-in-out infinite alternate;
    }

    @keyframes glow {
        from { filter: drop-shadow(0 0 5px rgba(255, 107, 107, 0.5)); }
        to { filter: drop-shadow(0 0 20px rgba(78, 205, 196, 0.5)); }
    }

    .nav-links {
        display: flex;
        list-style: none;
        gap: 2rem;
    }

    .nav-links a {
        color: white;
        text-decoration: none;
        padding: 0.5rem 1rem;
        border-radius: 20px;
        transition: all 0.3s ease;
        position: relative;
        overflow: hidden;
    }

    .nav-links a:hover {
        background: rgba(255, 255, 255, 0.2);
        transform: translateY(-2px);
    }

    .hero {
        text-align: center;
        padding: 4rem 2rem;
        max-width: 1200px;
        margin: 0 auto;
    }

    .hero h1 {
        font-size: 3.5rem;
        margin-bottom: 1rem;
        animation: fadeInUp 1s ease;
    }

    .hero p {
        font-size: 1.2rem;
        opacity: 0.9;
        margin-bottom: 2rem;
        animation: fadeInUp 1s ease 0.3s both;
    }

    @keyframes fadeInUp {
        from {
            opacity: 0;
            transform: translateY(30px);
        }
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }

    .search-container {
        max-width: 600px;
        margin: 2rem auto;
        position: relative;
        animation: fadeInUp 1s ease 0.6s both;
    }

    .search-box {
        width: 100%;
        padding: 1rem 1.5rem;
        font-size: 1.1rem;
        border: none;
        border-radius: 50px;
        background: rgba(255, 255, 255, 0.9);
        color: #333;
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        transition: all 0.3s ease;
    }

    .search-box:focus {
        outline: none;
        transform: scale(1.02);
        box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
    }

    .categories {
        display: flex;
        justify-content: center;
        gap: 1rem;
        margin: 3rem 0;
        flex-wrap: wrap;
        padding: 0 2rem;
        animation: fadeInUp 1s ease 0.9s both;
    }

    .category-btn {
        padding: 0.8rem 2rem;
        background: rgba(255, 255, 255, 0.1);
        border: 2px solid rgba(255, 255, 255, 0.3);
        border-radius: 25px;
        color: white;
        cursor: pointer;
        transition: all 0.3s ease;
        font-size: 1rem;
        backdrop-filter: blur(5px);
    }

    .category-btn:hover, .category-btn.active {
        background: rgba(255, 255, 255, 0.2);
        transform: translateY(-3px);
        box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
    }

    .games-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
        gap: 2rem;
        max-width: 1200px;
        margin: 0 auto;
        padding: 2rem;
    }

    .game-card {
        background: rgba(255, 255, 255, 0.1);
        border-radius: 20px;
        overflow: hidden;
        backdrop-filter: blur(10px);
        border: 1px solid rgba(255, 255, 255, 0.2);
        transition: all 0.3s ease;
        cursor: pointer;
        animation: fadeInUp 1s ease both;
    }

    .game-card:hover {
        transform: translateY(-10px);
        box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
    }

    .game-image {
        width: 100%;
        height: 200px;
        background: linear-gradient(45deg, #ff9a9e, #fecfef);
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 3rem;
        position: relative;
        overflow: hidden;
    }

    .game-image::before {
        content: '';
        position: absolute;
        top: -50%;
        left: -50%;
        width: 200%;
        height: 200%;
        background: linear-gradient(45deg, transparent, rgba(255, 255, 255, 0.3), transparent);
        transform: rotate(45deg);
        animation: shimmer 3s infinite;
    }

    @keyframes shimmer {
        0% { transform: translateX(-100%) translateY(-100%) rotate(45deg); }
        100% { transform: translateX(100%) translateY(100%) rotate(45deg); }
    }

    .game-info {
        padding: 1.5rem;
    }

    .game-title {
        font-size: 1.3rem;
        font-weight: bold;
        margin-bottom: 0.5rem;
    }

    .game-description {
        opacity: 0.8;
        font-size: 0.9rem;
        line-height: 1.4;
        margin-bottom: 1rem;
    }

    .play-btn {
        width: 100%;
        padding: 0.8rem;
        background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
        border: none;
        border-radius: 10px;
        color: white;
        font-size: 1rem;
        font-weight: bold;
        cursor: pointer;
        transition: all 0.3s ease;
    }

    .play-btn:hover {
        transform: scale(1.05);
        box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
    }

    .footer {
        background: rgba(0, 0, 0, 0.3);
        text-align: center;
        padding: 2rem;
        margin-top: 4rem;
    }

    @media (max-width: 768px) {
        .hero h1 {
            font-size: 2.5rem;
        }
        
        .nav-links {
            display: none;
        }
        
        .categories {
            gap: 0.5rem;
        }
        
        .category-btn {
            padding: 0.6rem 1.5rem;
            font-size: 0.9rem;
        }
    }

    .modal {
        display: none;
        position: fixed;
        z-index: 1000;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.8);
        backdrop-filter: blur(5px);
    }

    .modal-content {
        position: relative;
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        margin: 5% auto;
        padding: 2rem;
        width: 90%;
        max-width: 800px;
        border-radius: 20px;
        box-shadow: 0 20px 60px rgba(0, 0, 0, 0.5);
    }

    .close {
        color: white;
        float: right;
        font-size: 2rem;
        font-weight: bold;
        cursor: pointer;
        line-height: 1;
    }

    .close:hover {
        opacity: 0.7;
    }

    .game-frame {
        width: 100%;
        height: 500px;
        border: none;
        border-radius: 10px;
        margin-top: 1rem;
        background: white;
    }
</style>
```

</head>
<body>
    <header class="header">
        <nav class="nav-container">
            <div class="logo">🎮 GameZone</div>
            <ul class="nav-links">
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#juegos">Juegos</a></li>
                <li><a href="#categorias">Categorías</a></li>
                <li><a href="#contacto">Contacto</a></li>
            </ul>
        </nav>
    </header>

```
<main>
    <section class="hero" id="inicio">
        <h1>🎮 Juegos Desbloqueados</h1>
        <p>Disfruta de los mejores juegos online sin restricciones. ¡Diversión garantizada!</p>
        
        <div class="search-container">
            <input type="text" class="search-box" placeholder="🔍 Busca tu juego favorito..." id="searchInput">
        </div>
    </section>

    <section class="categories" id="categorias">
        <button class="category-btn active" data-category="todos">Todos</button>
        <button class="category-btn" data-category="accion">Acción</button>
        <button class="category-btn" data-category="puzzle">Puzzle</button>
        <button class="category-btn" data-category="deportes">Deportes</button>
        <button class="category-btn" data-category="estrategia">Estrategia</button>
        <button class="category-btn" data-category="aventura">Aventura</button>
    </section>

    <section class="games-grid" id="juegos">
        <!-- MAS CHIDOS -->
        <div class="game-card" data-category="aventura" data-game="mario3d">
            <div class="game-image">🍄</div>
            <div class="game-info">
                <h3 class="game-title">Mario 3D - ¡Más Popular!</h3>
                <p class="game-description">El icónico Mario en 3D. Aventuras increíbles te esperan en este mundo mágico.</p>
                <button class="play-btn">Jugar Ahora</button>
            </div>
        </div>

        <div class="game-card" data-category="accion" data-game="templerun">
            <div class="game-image">🏃</div>
            <div class="game-info">
                <h3 class="game-title">Temple Run - ¡Más Popular!</h3>
                <p class="game-description">Corre sin parar por templos antiguos. ¡Esquiva obstáculos y recolecta monedas!</p>
                <button class="play-btn">Jugar Ahora</button>
            </div>
        </div>

        <div class="game-card" data-category="accion" data-game="gamesop">
            <div class="game-image">🎮</div>
            <div class="game-info">
                <h3 class="game-title">Games Op</h3>
                <p class="game-description">Colección de juegos increíbles. Variedad y diversión garantizada.</p>
                <button class="play-btn">Jugar Ahora</button>
            </div>
        </div>

        <!-- RANDOM -->
        <div class="game-card" data-category="accion" data-game="randomgame">
            <div class="game-image">🎯</div>
            <div class="game-info">
                <h3 class="game-title">Random Games</h3>
                <p class="game-description">Descubre juegos al azar. Siempre algo nuevo y emocionante que probar.</p>
                <button class="play-btn">Jugar Ahora</button>
            </div>
        </div>

        <div class="game-card" data-category="aventura" data-game="mario2d">
            <div class="game-image">🍄</div>
            <div class="game-info">
                <h3 class="game-title">Mario 2D</h3>
                <p class="game-description">El clásico Mario Bros en 2D. Nostalgia pura con la mejor jugabilidad.</p>
                <button class="play-btn">Jugar Ahora</button>
            </div>
        </div>

        <div class="game-card" data-category="accion" data-game="classroom6x">
            <div class="game-image">🏫</div>
            <div class="game-info">
                <h3 class="game-title">Classroom6x</h3>
                <p class="game-description">Juegos especiales para el aula. Algunos pueden estar bloqueados.</p>
                <button class="play-btn">Jugar Ahora</button>
            </div>
        </div>

        <div class="game-card" data-category="accion" data-game="game76">
            <div class="game-image">🕹️</div>
            <div class="game-info">
                <h3 class="game-title">Game76</h3>
                <p class="game-description">Mega colección de 76 juegos desbloqueados. ¡Diversión sin límites!</p>
                <button class="play-btn">Jugar Ahora</button>
            </div>
        </div>
    </section>
</main>

<!-- Modal para juegos -->
<div id="gameModal" class="modal">
    <div class="modal-content">
        <span class="close">&times;</span>
        <h2 id="modalTitle">Cargando juego...</h2>
        <div id="gameContainer">
            <p>El juego se está cargando...</p>
        </div>
    </div>
</div>

<footer class="footer" id="contacto">
    <p>&copy; 2025 Juegos Desbloqueados. Todos los derechos reservados.</p>
    <p>¡Diversión sin límites para todos!</p>
</footer>

<script>
    // Variables globales
    const games = document.querySelectorAll('.game-card');
    const categoryBtns = document.querySelectorAll('.category-btn');
    const searchInput = document.getElementById('searchInput');
    const modal = document.getElementById('gameModal');
    const closeModal = document.querySelector('.close');
    const modalTitle = document.getElementById('modalTitle');
    const gameContainer = document.getElementById('gameContainer');

    // Animaciones al cargar
    window.addEventListener('load', () => {
        games.forEach((game, index) => {
            game.style.animationDelay = `${index * 0.1}s`;
        });
    });

    // Filtros por categoría
    categoryBtns.forEach(btn => {
        btn.addEventListener('click', () => {
            // Remover clase activa de todos los botones
            categoryBtns.forEach(b => b.classList.remove('active'));
            // Agregar clase activa al botón clickeado
            btn.classList.add('active');
            
            const category = btn.dataset.category;
            
            games.forEach(game => {
                if (category === 'todos' || game.dataset.category === category) {
                    game.style.display = 'block';
                    game.style.animation = 'fadeInUp 0.5s ease both';
                } else {
                    game.style.display = 'none';
                }
            });
        });
    });

    // Buscador
    searchInput.addEventListener('input', (e) => {
        const searchTerm = e.target.value.toLowerCase();
        
        games.forEach(game => {
            const title = game.querySelector('.game-title').textContent.toLowerCase();
            const description = game.querySelector('.game-description').textContent.toLowerCase();
            
            if (title.includes(searchTerm) || description.includes(searchTerm)) {
                game.style.display = 'block';
            } else {
                game.style.display = 'none';
            }
        });
    });

    // Abrir juegos en modal
    games.forEach(game => {
        const playBtn = game.querySelector('.play-btn');
        playBtn.addEventListener('click', () => {
            const gameTitle = game.querySelector('.game-title').textContent;
            const gameType = game.dataset.game;
            
            modalTitle.textContent = gameTitle;
            showGame(gameType);
            modal.style.display = 'block';
            document.body.style.overflow = 'hidden';
        });
    });

    // Cerrar modal
    closeModal.addEventListener('click', () => {
        modal.style.display = 'none';
        document.body.style.overflow = 'auto';
        gameContainer.innerHTML = '<p>El juego se está cargando...</p>';
    });

    window.addEventListener('click', (e) => {
        if (e.target === modal) {
            modal.style.display = 'none';
            document.body.style.overflow = 'auto';
            gameContainer.innerHTML = '<p>El juego se está cargando...</p>';
        }
    });

    // Función para mostrar juegos
    function showGame(gameType) {
        // URLs reales de los juegos
        const gameUrls = {
            // MAS CHIDOS
            'mario3d': 'https://auguhhcbxstberc/knhelmann.com/mario/',
            'templerun': 'https://games.engineering.com/temple-run-2/index.html',
            'gamesop': 'https://unblocked-games.s3.amazonaws.com/index.html',
            
            // RANDOM
            'randomgame': 'https://www.engineering.com/games/',
            'mario2d': 'https://supermariobrosonline.github.io/',
            'classroom6x': 'https://sites.google.com/view/classroom6x/',
            'game76': 'https://sites.google.com/view/unblocked-game76/home'
        };

        const gameUrl = gameUrls[gameType] || '#';
        
        gameContainer.innerHTML = `
            <iframe src="${gameUrl}" class="game-frame" title="${gameType} game"></iframe>
            <p style="margin-top: 1rem; text-align: center; opacity: 0.8;">
                Si el juego no carga, prueba refrescando la página o usando otro navegador.
            </p>
        `;
    }

    // Efectos de scroll suave
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function (e) {
            e.preventDefault();
            const target = document.querySelector(this.getAttribute('href'));
            if (target) {
                target.scrollIntoView({
                    behavior: 'smooth',
                    block: 'start'
                });
            }
        });
    });

    // Efecto parallax suave
    window.addEventListener('scroll', () => {
        const scrolled = window.pageYOffset;
        const header = document.querySelector('.header');
        
        if (scrolled > 100) {
            header.style.background = 'rgba(0, 0, 0, 0.5)';
        } else {
            header.style.background = 'rgba(0, 0, 0, 0.3)';
        }
    });

    // Animación de entrada para las cards
    const observerOptions = {
        threshold: 0.1,
        rootMargin: '0px 0px -50px 0px'
    };

    const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                entry.target.style.animationPlayState = 'running';
            }
        });
    }, observerOptions);

    games.forEach(game => {
        observer.observe(game);
    });
</script>
```

</body>
</html>
