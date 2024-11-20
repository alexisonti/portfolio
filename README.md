<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Página Personal</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* Estilos generales */
        body {
            margin: 0;
            padding: 0;
            height: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
            background-image: url("fondo de pagina.jpg");
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            background-attachment: fixed;
            font-family: Arial, sans-serif;
            color: #fff;
            text-align: center;
        }

        /* Contenedor de la barra superior para los íconos con fondo negro semi-transparente */
        .social-bar {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: rgba(0, 0, 0, 0.6); /* Fondo negro semi-transparente */
            padding: 10px 0;
            z-index: 10; /* Asegura que esté por encima del contenido */
            display: flex;
            justify-content: center; /* Centra los íconos */
        }

        .social-icons {
            display: flex;
            gap: 15px; /* Espacio entre íconos */
        }

        .social-icons a {
            display: block;
            width: 40px;
            height: 40px;
        }

        .social-icons img {
            width: 100%;
            height: 100%;
            border-radius: 8px; /* Bordes redondeados */
            cursor: pointer;
        }

        /* Contenedor principal */
        .contenido {
            background-color: rgba(0, 0, 0, 0.6);
            border-radius: 15px;
            padding: 20px;
            margin: 20px auto;
            width: 90%;
            max-width: 800px;
            margin-top: 80px; /* Desplazar contenido hacia abajo, después de la barra */
        }

        /* Imagen principal */
        img {
            max-width: 300px;
            width: 100%;
            height: auto;
            border-radius: 10px;
            display: block;
            margin: 0 auto 10px auto;
        }

        /* Títulos */
        h1 {
            margin: 0 0 10px;
        }

        h2 {
            margin: 10px 0;
        }

        /* Párrafo */
        p {
            font-size: 18px;
            margin: 10px 0;
        }

        /* About Me en negrita */
        .about-me-title {
            font-weight: bold;
            margin-bottom: 10px;
            font-size: 20px;
        }

        /* Programador Junior */
        .programador-junior {
            font-size: 14px; /* Tamaño más pequeño */
            color: #ccc; /* Color gris para distinción */
            margin-top: 5px; /* Espacio por encima */
        }

        /* Skills */
        .skills {
            background-color: rgba(0, 0, 0, 0.6);
            border-radius: 15px;
            padding: 15px; /* Más pequeño */
            margin-top: 20px;
            width: 60%; /* Más angosto */
            max-width: 500px; /* Ancho máximo reducido */
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .skills-images {
            display: flex;
            justify-content: center;
            gap: 10px; /* Reduce el espacio entre imágenes */
            margin-top: 10px; /* Más compacto */
        }

        .skills-images img {
            width: 50px;
            height: 50px;
            border-radius: 8px;
            cursor: pointer;
        }

        /* Proyectos */
        .projects {
            background-color: rgba(0, 0, 0, 0.6);
            border-radius: 15px;
            padding: 20px;
            margin-top: 20px;
            width: 90%;
            max-width: 800px;
            text-align: center;
        }

        .project-card {
            background: rgba(255, 255, 255, 0.2);
            padding: 15px;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        .project-card img {
            width: 100%;
            max-width: 300px;
            height: auto;
            border-radius: 8px;
            display: block;
            margin: 0 auto;
        }

        .project-card a {
            color: #ffd700;
            text-decoration: none;
            font-weight: bold;
        }

        /* Formulario de Contacto */
        form {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 10px;
            margin-top: 20px;
        }

        form input, form textarea, form button {
            width: 100%;
            max-width: 400px;
            padding: 10px;
            border: none;
            border-radius: 5px;
        }

        form button {
            background-color: #ffd700;
            color: #000;
            font-weight: bold;
            cursor: pointer;
        }

        form button:hover {
            background-color: #ffa500;
        }
    </style>
</head>
<body>
    <!-- Barra superior con fondo negro semi-transparente -->
    <div class="social-bar">
        <div class="social-icons">
            <a href="https://www.linkedin.com/in/alexisontiveros/" target="_blank">
                <img src="linkedin.png" alt="LinkedIn">
            </a>
            <a href="https://github.com/alexisonti" target="_blank">
                <img src="GitHub.png" alt="GitHub">
            </a>
            <a href="alexis.ontiveros.tejada@gmail.com">
                <img src="gmail.png" alt="Gmail">
            </a>
        </div>
    </div>

    <!-- Imagen central con título -->
    <div class="contenido">
        <img src="foto para web.jpeg" alt="Mi Imagen Central">
        <h1>Alexis Ontiveros</h1>
        <p class="programador-junior">Programador Junior</p> <!-- Agregado aquí -->
    </div>

    <!-- Sobre mí -->
    <div class="contenido">
        <h2 class="about-me-title">About Me</h2>
        <p>
            Soy de Argentina, estoy estudiando Ingeniería en Sistemas en la UTN Córdoba y actualmente trabajo como SA Operator.
        </p>
    </div>

    <!-- Skills -->
    <div class="contenido skills">
        <h2>Skills</h2>
        <div class="skills-images">
            <img src="python.png" alt="Python">
            <img src="sql.png" alt="SQL">
            <img src="html.png" alt="HTML">
        </div>
    </div>

    <!-- Proyectos -->
    <div class="projects">
        <h2>My Projects</h2>
        <div class="project-card">
            <img src="project1.png" alt="Project 1">
            <h3>Project 1</h3>
            <p>Descripción breve del proyecto.</p>
            <a href="https://github.com/username/project1" target="_blank">View on GitHub</a>
        </div>
        <div class="project-card">
            <img src="project2.png" alt="Project 2">
            <h3>Project 2</h3>
            <p>Descripción breve del proyecto.</p>
            <a href="https://github.com/username/project2" target="_blank">View on GitHub</a>
        </div>
    </div>

    <!-- Formulario de Contacto -->
    <div class="contenido">
        <h2>Contact</h2>
        <form action="https://formspree.io/f/your-id" method="POST">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" placeholder="Your Message" rows="5" required></textarea>
            <button type="submit">Send</button>
        </form>
    </div>
</body>
</html>
