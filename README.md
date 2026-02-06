<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Perfil Personal</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
            color: #f0f0f0;
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 1000px;
            margin: 0 auto;
        }

        header {
            text-align: center;
            padding: 30px 0;
            margin-bottom: 30px;
        }

        h1 {
            font-size: 2.8rem;
            background: linear-gradient(to right, #ff8a00, #da1b60);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 10px;
            text-shadow: 0 0 15px rgba(218, 27, 96, 0.3);
        }

        .tagline {
            font-size: 1.2rem;
            color: #b0b0d0;
            font-style: italic;
        }

        section {
            background: rgba(20, 18, 40, 0.8);
            border-radius: 15px;
            padding: 25px;
            margin-bottom: 30px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: transform 0.3s ease;
        }

        section:hover {
            transform: translateY(-5px);
        }

        h2 {
            color: #ff8a00;
            border-bottom: 2px solid #da1b60;
            padding-bottom: 10px;
            margin-bottom: 20px;
            font-size: 1.8rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        h2 i {
            font-size: 1.5rem;
        }

        .description {
            line-height: 1.6;
            font-size: 1.1rem;
        }

        .music-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }

        .music-card {
            background: rgba(30, 28, 50, 0.9);
            border-radius: 10px;
            overflow: hidden;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 138, 0, 0.2);
        }

        .music-card:hover {
            border-color: #ff8a00;
            box-shadow: 0 5px 15px rgba(255, 138, 0, 0.2);
        }

        .music-img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            border-bottom: 2px solid #da1b60;
        }

        .music-info {
            padding: 15px;
        }

        .music-title {
            font-size: 1.3rem;
            color: #ffcc00;
            margin-bottom: 5px;
        }

        .music-artist {
            color: #b0b0d0;
            font-size: 1rem;
            margin-bottom: 10px;
        }

        .music-link {
            display: inline-block;
            background: #da1b60;
            color: white;
            padding: 8px 15px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: background 0.3s ease;
        }

        .music-link:hover {
            background: #ff8a00;
        }

        .projects-container {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .project-item {
            background: rgba(30, 28, 50, 0.7);
            padding: 15px;
            border-radius: 10px;
            border-left: 4px solid #ff8a00;
        }

        .project-title {
            color: #ffcc00;
            font-size: 1.2rem;
            margin-bottom: 8px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .project-desc {
            color: #d0d0e0;
            line-height: 1.5;
        }

        footer {
            text-align: center;
            padding: 20px;
            color: #8888aa;
            font-size: 0.9rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            margin-top: 20px;
        }

        @media (max-width: 768px) {
            .music-grid {
                grid-template-columns: 1fr;
            }
            
            h1 {
                font-size: 2.2rem;
            }
            
            section {
                padding: 20px;
            }
        }

        /* Efectos de animación */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        section {
            animation: fadeIn 0.8s ease-out;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Mi Perfil Personal</h1>
            <p class="tagline">Desarrollador • Músico • Creador de contenido</p>
        </header>

        <!-- Sección de Descripción -->
        <section id="descripcion">
            <h2><i class="fas fa-user"></i> Sobre Mí</h2>
            <div class="description">
                <p>¡Hola! Soy un apasionado por la tecnología, la música y la creatividad digital. Me encanta aprender nuevas habilidades y compartir mis proyectos con la comunidad. En mi tiempo libre disfruto explorando nuevas herramientas de desarrollo y descubriendo música de todos los géneros.</p>
                <p>Este espacio es mi rincón personal en la web, donde comparto mis gustos musicales y los proyectos en los que estoy trabajando. ¡Siéntete libre de explorar y conectar conmigo!</p>
            </div>
        </section>

        <!-- Sección de Música Favorita -->
        <section id="musica">
            <h2><i class="fas fa-music"></i> Mi Música Favorita</h2>
            <div class="music-grid">
                <!-- Canción 1 -->
                <div class="music-card">
                    <img src="https://images.genius.com/06c4f4edeb0d45947980e34897a0342d.1000x1000x1.jpg" alt="Portada de Ella Y Tú" class="music-img">
                    <div class="music-info">
                        <h3 class="music-title">Ella Y Tú</h3>
                        <p class="music-artist">Juan Manuel Lebron</p>
                        <a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ" target="_blank" class="music-link">
                            <i class="fab fa-youtube"></i> Escuchar en YouTube
                        </a>
                    </div>
                </div>

                <!-- Canción 2 (ejemplo) -->
                <div class="music-card">
                    <img src="https://i.scdn.co/image/ab67616d0000b27384f7de4f3a517b3d8c2c4c0a" alt="Portada de otra canción" class="music-img">
                    <div class="music-info">
                        <h3 class="music-title">Nombre de Canción</h3>
                        <p class="music-artist">Artista Ejemplo</p>
                        <a href="#" target="_blank" class="music-link">
                            <i class="fab fa-spotify"></i> Escuchar en Spotify
                        </a>
                    </div>
                </div>

                <!-- Canción 3 (ejemplo) -->
                <div class="music-card">
                    <img src="https://upload.wikimedia.org/wikipedia/en/2/2e/Blinding_Lights_%28Official_Single_Cover%29.png" alt="Portada de ejemplo" class="music-img">
                    <div class="music-info">
                        <h3 class="music-title">Otra Canción Favorita</h3>
                        <p class="music-artist">Otro Artista</p>
                        <a href="#" target="_blank" class="music-link">
                            <i class="fas fa-headphones"></i> Escuchar en línea
                        </a>
                    </div>
                </div>
            </div>
        </section>

        <!-- Sección de Proyectos -->
        <section id="proyectos">
            <h2><i class="fas fa-code"></i> Mis Proyectos</h2>
            <div class="projects-container">
                <!-- Proyecto 1 -->
                <div class="project-item">
                    <h3 class="project-title"><i class="fas fa-globe"></i> Sitio Web Personal</h3>
                    <p class="project-desc">Desarrollo de un portafolio web interactivo para mostrar mis trabajos de diseño y programación. Utilizando HTML, CSS y JavaScript.</p>
                </div>

                <!-- Proyecto 2 -->
                <div class="project-item">
                    <h3 class="project-title"><i class="fas fa-mobile-alt"></i> App de Tareas</h3>
                    <p class="project-desc">Aplicación móvil para gestión de tareas diarias con recordatorios y sincronización en la nube. Desarrollada con React Native.</p>
                </div>

                <!-- Proyecto 3 -->
                <div class="project-item">
                    <h3 class="project-title"><i class="fas fa-gamepad"></i> Juego en JavaScript</h3>
                    <p class="project-desc">Creación de un juego de plataformas 2D utilizando el canvas de HTML5 y JavaScript puro. Actualmente en fase de desarrollo.</p>
                </div>

                <!-- Proyecto 4 -->
                <div class="project-item">
                    <h3 class="project-title"><i class="fas fa-robot"></i> Bot de Discord</h3>
                    <p class="project-desc">Desarrollo de un bot multifuncional para servidores de Discord con comandos de moderación, música y utilidades.</p>
                </div>
            </div>
        </section>

        <footer>
            <p>© 2023 Mi Perfil Personal. Todos los derechos reservados.</p>
            <p>Diseñado con ❤️ y código.</p>
        </footer>
    </div>

    <script>
        // Animación suave para los enlaces
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 20,
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Efecto de aparición al hacer scroll
        const observerOptions = {
            threshold: 0.1
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if(entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        // Aplicar a las secciones
        document.querySelectorAll('section').forEach(section => {
            section.style.opacity = '0';
            section.style.transform = 'translateY(20px)';
            section.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
            observer.observe(section);
        });
    </script>
</body>
</html>
