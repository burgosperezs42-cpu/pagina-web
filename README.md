<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¡Dos super contenidos llenos de aventuras y aprendizaje!</title>
    <style>
        body {
            font-family: 'Nunito', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(to right, #ff5e62, #ff9966);
            color: #fff;
            overflow-x: hidden;
            animation: gradientAnimation 10s ease infinite;
        }

        .container {
            width: 80%;
            margin: 30px auto;
            background-color: rgba(255, 255, 255, 0.15);
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 0 30px rgba(0, 0, 0, 0.4);
            backdrop-filter: blur(7px);
            position: relative;
            overflow: hidden;
            animation: fadeIn 1.5s ease-out;
        }

        h1 {
            color: #fff;
            text-align: center;
            margin-bottom: 40px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            animation: neonText 2s ease-in-out infinite alternate;
        }

        .page {
            display: none;
            padding: 30px;
            border-radius: 12px;
            animation: slideIn 1s ease-out;
        }

        .page.active {
            display: block;
        }

        button {
            background-color: #fff;
            color: #e44d26;
            padding: 15px 30px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            margin: 5px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
            font-weight: bold;
        }

        button:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.4);
        }

        img {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
            margin-bottom: 20px;
            animation: zoomIn 1.2s ease-out;
        }

        p {
            font-size: 1.1em;
            line-height: 1.6;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
        }

        /* Animaciones */
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateX(-30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        @keyframes zoomIn {
            from {
                transform: scale(0.8);
                opacity: 0;
            }
            to {
                transform: scale(1);
                opacity: 1;
            }
        }

        @keyframes neonText {
            from {
                text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5), 0 0 10px #fff, 0 0 20px #fff;
            }
            to {
                text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5), 0 0 5px #fff, 0 0 10px #fff;
            }
        }

        @keyframes gradientAnimation {
            0% {
                background-position: 0% 50%;
            }
            50% {
                background-position: 100% 50%;
            }
            100% {
                background-position: 0% 50%;
            }
        }

        /* Estilos adicionales */
        .button-container {
            text-align: center;
            margin-bottom: 30px;
        }

        .thanks-message {
            text-align: center;
            font-size: 1.3em;
            margin-top: 40px;
            animation: pulse 2s ease-in-out infinite;
        }

        @keyframes pulse {
            0% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.1);
            }
            100% {
                transform: scale(1);
            }
        }

        ul, ol {
            padding-left: 30px;
            margin-bottom: 20px;
        }

        li {
            margin-bottom: 8px;
            font-size: 1.05em;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
        }

        h2 {
            color: #fff;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        /* Estilos para la tabla */
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
            border-radius: 8px;
            overflow: hidden;
        }

        th, td {
            padding: 12px 15px;
            text-align: left;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        th {
            background-color: rgba(255, 255, 255, 0.1);
            font-weight: bold;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
        }

        tr:last-child td {
            border-bottom: none;
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
    <div class="container">
        <h1>¡Dos super contenidos llenos de aventuras y aprendizaje !</h1>

        <!-- Botones de navegación -->
        <div class="button-container">
            <button onclick="showPage('pagina1')">contenido 1: ¡Aprende y Diviértete!</button>
            <button onclick="showPage('pagina2')">contenido 2: ¡Explora el Mundo!</button>
        </div>

        <!-- Contenido de la Página 1 -->
        <div id="pagina1" class="page active">
            <h2>¡Bienvenido al Rincón del Saber!</h2>
            <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExaDY0a3c4aXAzc3Zmbm9xbXJ2aXJmc2F1eXN0b21vNnJpYjVqYiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT0xeJpnrWC4XWblEk/giphy.gif" alt="Animación 1">
            <p>¡Prepárate para una aventura llena de conocimientos! Aquí encontrarás datos curiosos, información útil y un montón de cosas interesantes para aprender. ¡No te lo pierdas!</p>

            <h3>Temas que te encantarán:</h3>
            <ul>
                <li>Historia Universal: ¡Viaja en el tiempo y descubre los secretos del pasado!</li>
                <li>Ciencia Asombrosa: ¡Explora los misterios del universo y la naturaleza!</li>
                <li>Tecnología del Futuro: ¡Descubre las innovaciones que transformarán el mundo!</li>
            </ul>

            <h3>Tabla de Datos Curiosos:</h3>
            <table>
                <thead>
                    <tr>
                        <th>Dato Curioso</th>
                        <th>Explicación</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>¿Sabías que...?</td>
                        <td>Las abejas pueden reconocer rostros humanos.</td>
                    </tr>
                    <tr>
                        <td>Increíble pero cierto:</td>
                        <td>El corazón de una ballena azul es tan grande que una persona podría nadar a través de sus arterias.</td>
                    </tr>
                    <tr>
                        <td>Un dato sorprendente:</td>
                        <td>En Marte, el sol se ve de color azul.</td>
                    </tr>
                </tbody>
            </table>
        </div>

        <!-- Contenido de la Página 2 -->
        <div id="pagina2" class="page">
            <h2>¡Atrévete a Explorar el Mundo!</h2>
            <img src="https://images.unsplash.com/photo-1469854523086-cc02fe5d8800?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8NXx8dHJhdmVsfGVufDB8fDB8fHx8MA%3D%3D&auto=format&fit=crop&w=500&q=60" alt="Montañas">
            <p>¡Embárcate en un viaje lleno de aventuras y descubrimientos! Aquí encontrarás información sobre lugares increíbles, culturas fascinantes y experiencias inolvidables. ¡Prepárate para explorar!</p>

            <h3>Destinos Imperdibles:</h3>
            <ol>
                <li>Machu Picchu, Perú: ¡Descubre la magia de la antigua ciudad inca!</li>
                <li>Gran Muralla China: ¡Camina por una de las maravillas del mundo!</li>
                <li>Santorini, Grecia: ¡Déjate enamorar por sus paisajes de ensueño!</li>
            </ol>

            <h3>Consejos para Viajeros:</h3>
            <ul>
                <li>Planifica con anticipación: ¡Reserva tus vuelos y alojamiento con tiempo!</li>
                <li>Aprende algunas frases básicas: ¡Comunícate con los locales en su idioma!</li>
                <li>Respeta la cultura local: ¡Sumérgete en las tradiciones y costumbres del lugar!</li>
            </ul>

            <h3>¿Qué esperas para comenzar tu próxima aventura?</h3>
        </div>

        <!-- Mensaje de agradecimiento -->
        <div class="thanks-message">
            ¡Gracias por participar! ¡que tengas un dia  lleno de aprendizaje y aventuras! 🎉
        </div>
    </div>

    <script>
        function showPage(pageId) {
            let pages = document.getElementsByClassName('page');
            for (let i = 0; i < pages.length; i++) {
                pages[i].classList.remove('active');
            }
            document.getElementById(pageId).classList.add('active');
        }
    </script>
</body>
</html>
