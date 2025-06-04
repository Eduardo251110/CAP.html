<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página Profesional</title>
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
            background-image: url('https://th.bing.com/th/id/OIP.OiWLVAweyawlVD7-gyT_5QHaEw?rs=1&pid=ImgDetMain');
            background-size: cover;
            background-position: center;
        }

        .slider {
            width: 100%;
            overflow: hidden;
            position: relative;
        }

        .slider img {
            width: 100%;
            display: none;
            position: absolute;
            top: 0;
            left: 0;
        }

        .slider img.active {
            display: block;
        }

        .container {
            max-width: 800px;
            margin: 50px auto;
            background: rgba(255, 255, 255, 0.95);
            padding: 40px;
            border-radius: 18px;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.2);
            text-align: center;
        }

        .container h1 {
            font-size: 3em;
            color: #2e7d32;
            margin-bottom: 10px;
            text-shadow: 1px 1px 4px rgba(0, 0, 0, 0.2);
        }

        .container p {
            font-size: 1.3em;
            color: #BE0032;
            margin-bottom: 20px;
        }

        .container img {
            max-width: 220px;
            height: auto;
            margin-bottom: 20px;
            border: 4px solid #BE0032;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.25);
            border-radius: 12px;
        }

        @keyframes bounce {
            0% { transform: translateY(0); }
            50% { transform: translateY(-10px) scale(1.05); }
            100% { transform: translateY(0); }
        }

        .plant-container img {
            transition: transform 0.3s ease;
        }

        .plant-container img:hover {
            animation: bounce 0.6s ease;
            box-shadow: 0px 12px 25px rgba(0, 128, 0, 0.5);
        }

        .moveable-image-container {
            position: relative;
            width: 300px;
            height: 300px;
            margin: 50px auto;
            background-color: #BE0032;
            border-radius: 10px;
            overflow: hidden;
        }

        .moveable-image {
            width: 100%;
            height: 100%;
            position: absolute;
            cursor: grab;
        }

        .plant-info {
            margin-top: 30px;
            padding: 20px;
            background: rgba(255, 255, 255, 0.8);
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        #fraseBox {
            position: fixed;
            left: 20px;
            top: 120px;
            background: rgba(255, 255, 255, 0.85);
            border: 2px solid #4caf50;
            border-radius: 12px;
            padding: 12px;
            max-width: 200px;
            z-index: 999;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            font-family: 'Poppins', sans-serif;
            text-align: left;
        }

        #fraseBox button {
            background-color: #BE0032;
            border: none;
            color: white;
            padding: 8px 12px;
            border-radius: 8px;
            cursor: pointer;
            font-size: 14px;
        }

        #fraseBox button:hover {
            background-color: #BE0032;
        }

        #fraseTexto {
            margin-top: 10px;
            font-size: 0.95em;
            color: #BE0032;
        }

        #login, #register {
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: rgba(255, 255, 255, 0.9);
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            width: 300px;
        }

        input[type="text"], input[type="password"] {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        button {
            padding: 10px 15px;
            background-color: #4caf50;
            border: none;
            color: white;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #BE0032;
        }
    </style>
</head>
<body>
    <div style="position: fixed; top: 20px; right: 20px; z-index: 1000;">
        <button onclick="showLoginForm()">Iniciar Sesión</button>
    </div>

    <div id="mainPage" style="display: none;">
        <div class="slider">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTiEsIj_kRklsvCJO1Bu-QbVaeRgk5Zd9SpMw&s" class="active" alt="Imagen 1">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQBqk4rKdj4LiYRkvH9msab3rIQn37ucMIyZg&s" alt="Imagen 2">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR2dGyf_mf25CGgXfxfMbtYhmIzFipsKcKTaw&s" alt="Imagen 3">
        </div>

        <div class="container">
            <h1>CAP</h1>
            <p>Curso De Atenciones Primarias.</p> 	
            <img src="https://www.ifrc.org/sites/default/files/styles/icon_block_thumbnail/public/2021-07/emblems-white-01.png?itok=NPntkkrx">
            <div class="plant-container">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQXLBYLZQXIcl2EvijiJ3We6n_kzZWCWNKgaw&s" alt="Planta 1">
                <img src="https://lirp.cdn-website.com/a979b4f7/dms3rep/multi/opt/gente-caminando-sentada-edificio-hospital-exterior-cristal-clinica-ciudad-ilustracion-vector-plano-ayuda-medica-emergencia-arquitectura-concepto-salud_74855-10130-640w.jpg" alt="Planta 2">
                <img src="https://us.123rf.com/450wm/lookua/lookua2305/lookua230500753/204154347-mano-vendada-de-primeros-auxilios.jpg?ver=6" alt="Planta 3">
            </div>
        </div>

        <div class="plant-info">
            <h2>Información sobre el CAP</h2>
            <p>El CAP se centra en enseñar lo basico para los jovenes de la actualidad</p>
            <p>porque vimos necesario el que las personas tuvieran este conocimiento para las situaciones en nuestro entorno.</p>
        </div>

        <div class="moveable-image-container">
            <img src="https://img.freepik.com/vector-gratis/ambulancia-emergencia-sobre-fondo-blanco_1308-95157.jpg?semt=ais_hybrid&w=740" alt="Planta Móvil" class="moveable-image" id="moveableImage">
        </div>
	<div class="presentation">
	<a href="https://docs.google.com/presentation/d/e/2PACX-1vSbQlNnXTQfjrNcT4foj_IqfN-Tv9lLBlArGlxqN1izFm_Jqv0ZtkZbo7ZOUyONAETolnUGPC-DrMoK/pub?start=false&loop=false&delayms=3000" download>
  <button style="padding: 10px 20px; background-color: #28a745; color: white; border: none; border-radius: 5px; cursor: pointer;">
    Presentación
  </button>
</a>

	</object>
	<a href="https://docs.google.com/presentation/d/e/2PACX-1vSjAAIfY5F9zPtNciLxAcxQpL7qmI7aVNLsUlMY7IoO0yfB4X0JKsEB4WdKCho36JnnCqJNcTkjj25b/pub?start=false&loop=false&delayms=3000" download>
  <button style="padding: 10px 20px; background-color: #28a745; color: white; border: none; border-radius: 5px; cursor: pointer;">
    Manual de Primeros Auxilios
  </button>
</a>

	</object>
	</div>
	 
    </div>


	<div class="container" style="margin-bottom: 50px;">
        <h2>Comentarios</h2>
        <textarea id="comentarioTexto" placeholder="Escribe tu comentario aquí..." rows="4" style="width: 100%; padding: 10px; border-radius: 8px; border: 1px solid #ccc;"></textarea>
        <br><br>
        <button onclick="agregarComentario()">Enviar Comentario</button>
        <div id="comentariosLista" style="margin-top: 20px; text-align: left;"></div>
    </div>

    <script>
        function agregarComentario() {
            const texto = document.getElementById("comentarioTexto").value.trim();
            if (texto) {
                const div = document.createElement("div");
                div.style.marginBottom = "15px";
                div.style.padding = "10px";
                div.style.border = "1px solid #ccc";
                div.style.borderRadius = "8px";
                div.style.backgroundColor = "#f9f9f9";
                div.innerText = texto;
                document.getElementById("comentariosLista").appendChild(div);
                document.getElementById("comentarioTexto").value = "";
            } else {
                alert("Por favor escribe un comentario antes de enviar.");
            }
        }
    </script>
	    <!-- Login y Registro -->
    <div id="login">
        <h2>Iniciar sesión</h2>
        <input type="text" placeholder="Usuario" id="loginUser">
        <input type="password" placeholder="Contraseña" id="loginPass">
        <button onclick="login()">Iniciar Sesión</button>
        <p>¿No tienes cuenta? <a href="javascript:showRegisterForm()">Regístrate</a></p>
    </div>

    <div id="register">
        <h2>Registrar cuenta</h2>
        <input type="text" placeholder="Usuario" id="registerUser">
        <input type="password" placeholder="Contraseña" id="registerPass">
        <button onclick="register()">Registrar</button>
        <p>¿Ya tienes cuenta? <a href="javascript:showLoginForm()">Inicia sesión</a></p>
    </div>

    <div id="fraseBox">
        <button onclick="mostrarFrase()">🚑 Ver Consejo</button>
        <p id="fraseTexto"></p>
    </div>

    <script>
        let index = 0;
        function changeImage() {
            let images = document.querySelectorAll('.slider img');
            images[index].classList.remove('active');
            index = (index + 1) % images.length;
            images[index].classList.add('active');
        }
        setInterval(changeImage, 3000);

        let moveableImage = document.getElementById('moveableImage');
        let isDragging = false;
        let offsetX, offsetY;

        moveableImage.addEventListener('mousedown', (e) => {
            isDragging = true;
            offsetX = e.clientX - moveableImage.offsetLeft;
            offsetY = e.clientY - moveableImage.offsetTop;
            moveableImage.style.cursor = 'grabbing';
        });

        document.addEventListener('mousemove', (e) => {
            if (isDragging) {
                moveableImage.style.left = `${e.clientX - offsetX}px`;
                moveableImage.style.top = `${e.clientY - offsetY}px`;
            }
        });

        document.addEventListener('mouseup', () => {
            isDragging = false;
            moveableImage.style.cursor = 'grab';
        });

        const frases = [
            "Revisa el entorno antes de actuar: asegúrate de que es seguro.",
            "Llama a emergencias antes de intervenir si la situación es grave.",
            "No muevas a una persona inconsciente a menos que esté en peligro.",
            "Presiona directamente sobre una herida sangrante para detener el sangrado.",
            "En caso de quemadura, enfría la zona con agua durante al menos 10 minutos.",
            "Si alguien no respira, inicia RCP si estás capacitado para ello.",
            "Mantén la calma: tu tranquilidad ayuda a la víctima.",
            "Usa guantes si es posible para evitar el contacto con fluidos."
        ];

        function mostrarFrase() {
            document.getElementById('fraseTexto').textContent = frases[Math.floor(Math.random() * frases.length)];
        }

        function showLoginForm() {
            document.getElementById('login').style.display = 'block';
            document.getElementById('register').style.display = 'none';
        }

        function showRegisterForm() {
            document.getElementById('login').style.display = 'none';
            document.getElementById('register').style.display = 'block';
        }

        function login() {
            document.getElementById('login').style.display = 'none';
            document.getElementById('mainPage').style.display = 'block';
        }

        function register() {
            document.getElementById('register').style.display = 'none';
            document.getElementById('mainPage').style.display = 'block';
        }
    </script>
</body>
</html>
