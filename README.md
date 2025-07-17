# morchis.html
Morchi
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Mi Morchis ❤</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: linear-gradient(135deg, #f5e6d8 0%, #e2c9a8 100%);
            font-family: 'Poppins', sans-serif;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            position: relative;
            padding: 20px;
        }
        
        .container {
            width: 100%;
            max-width: 800px;
            background: rgba(255, 255, 255, 0.85);
            border-radius: 25px;
            box-shadow: 0 15px 50px rgba(0, 0, 0, 0.2);
            backdrop-filter: blur(10px);
            overflow: hidden;
            position: relative;
            z-index: 10;
            padding: 40px 30px;
            text-align: center;
        }
        
        h1 {
            font-family: 'Dancing Script', cursive;
            font-size: 4.2rem;
            color: #d14b4b;
            margin: 20px 0;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
            animation: latido 2s infinite alternate;
        }
        
        @keyframes latido {
            0% { transform: scale(1); }
            100% { transform: scale(1.05); }
        }
        
        .heart-btn-container {
            position: relative;
            display: inline-block;
            margin: 40px 0;
        }
        
        .heart-btn {
            padding: 22px 50px;
            font-size: 1.8rem;
            background: linear-gradient(45deg, #ff6b6b, #ff8e8e);
            color: white;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            box-shadow: 0 8px 25px rgba(255, 107, 107, 0.4);
            transition: all 0.4s ease;
            font-weight: 600;
            letter-spacing: 1px;
            position: relative;
            z-index: 2;
        }
        
        .heart-btn:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 12px 30px rgba(255, 107, 107, 0.6);
        }
        
        .heart-btn:active {
            transform: translateY(0) scale(0.98);
        }
        
        .click-counter {
            position: absolute;
            top: -15px;
            right: -15px;
            background: #ffcc33;
            color: #5e3023;
            font-weight: bold;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.4rem;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            z-index: 3;
            animation: pulse 1.5s infinite;
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }
        
        .message-container {
            min-height: 180px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 30px 0;
            padding: 20px;
        }
        
        .message-box {
            background: linear-gradient(45deg, #ffebee, #ffe8d6);
            border-radius: 20px;
            padding: 30px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
            display: inline-block;
            max-width: 90%;
            opacity: 0;
            transform: translateY(20px);
            transition: all 0.7s ease;
        }
        
        .message-box.show {
            opacity: 1;
            transform: translateY(0);
        }
        
        .message-text {
            font-size: 1.8rem;
            font-weight: 600;
            color: #5e3023;
            line-height: 1.5;
        }
        
        .signature {
            font-family: 'Dancing Script', cursive;
            font-size: 2.5rem;
            color: #d14b4b;
            margin-top: 30px;
            padding: 15px 30px;
            background: rgba(255, 255, 255, 0.6);
            display: inline-block;
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }
        
        /* Elementos decorativos */
        .decorative-element {
            position: absolute;
            z-index: 1;
            pointer-events: none;
            animation: float 8s ease-in-out infinite alternate;
        }
        
        .mushroom {
            font-size: 3rem;
            filter: drop-shadow(0 4px 6px rgba(0, 0, 0, 0.2));
            animation: balanceo 8s ease-in-out infinite alternate;
        }
        
        .moth {
            font-size: 2.5rem;
            filter: drop-shadow(0 0 8px rgba(255, 215, 0, 0.4));
            animation: vuelo-magico 12s linear infinite;
        }
        
        .hearts {
            position: absolute;
            font-size: 2rem;
            color: #ff6b6b;
            animation: flotar 5s linear infinite;
            z-index: 1;
            opacity: 0;
        }
        
        /* Animaciones */
        @keyframes float {
            0% { transform: translateY(0) rotate(0deg); }
            100% { transform: translateY(-20px) rotate(5deg); }
        }
        
        @keyframes balanceo {
            0% { transform: rotate(-5deg) translateY(0); }
            100% { transform: rotate(5deg) translateY(-15px); }
        }
        
        @keyframes vuelo-magico {
            0% { transform: translate(0, 0) rotate(0deg) scale(1); }
            25% { transform: translate(50px, -30px) rotate(15deg) scale(1.1); }
            50% { transform: translate(20px, -50px) rotate(0deg) scale(0.9); }
            75% { transform: translate(-40px, -30px) rotate(-15deg) scale(1.05); }
            100% { transform: translate(0, 0) rotate(0deg) scale(1); }
        }
        
        @keyframes flotar {
            0% { transform: translateY(0) rotate(0deg); opacity: 1; }
            100% { transform: translateY(-100vh) rotate(360deg); opacity: 0; }
        }
        
        @keyframes aparecer {
            0% { opacity: 0; transform: scale(0.5); }
            100% { opacity: 1; transform: scale(1); }
        }
        
        @keyframes twinkle {
            0% { opacity: 0.3; transform: scale(0.8); }
            100% { opacity: 1; transform: scale(1.2); }
        }
        
        @media (max-width: 768px) {
            h1 { font-size: 3.2rem; }
            .heart-btn { font-size: 1.5rem; padding: 18px 40px; }
            .message-text { font-size: 1.5rem; }
            .signature { font-size: 2rem; }
            .click-counter { width: 40px; height: 40px; font-size: 1.2rem; }
        }
        
        @media (max-width: 480px) {
            h1 { font-size: 2.5rem; }
            .heart-btn { font-size: 1.3rem; padding: 15px 30px; }
            .message-text { font-size: 1.3rem; }
            .signature { font-size: 1.8rem; }
            .click-counter { width: 35px; height: 35px; font-size: 1rem; top: -12px; right: -12px; }
        }
    </style>
</head>
<body>
    <!-- Elementos decorativos -->
    <div class="decorative-element mushroom" style="bottom: 20px; left: 30px;">🍄</div>
    <div class="decorative-element mushroom" style="top: 50px; right: 40px; transform: rotate(15deg)">🍄</div>
    <div class="decorative-element mushroom" style="top: 20px; left: 10%;">🍄</div>
    <div class="decorative-element mushroom" style="bottom: 15%; right: 10%;">🍄</div>
    
    <div class="decorative-element moth" style="top: 20px; left: 15%;">🦋</div>
    <div class="decorative-element moth" style="bottom: 30%; right: 5%;">🦋</div>
    <div class="decorative-element moth" style="top: 25%; right: 20px;">🦋</div>
    <div class="decorative-element moth" style="bottom: 10%; left: 25%;">🦋</div>
    
    <div class="decorative-element" style="top: 15%; left: 5%; font-size: 3rem; color: #ff8e8e; animation: float 10s ease-in-out infinite alternate-reverse;">🍂</div>
    <div class="decorative-element" style="bottom: 20%; right: 8%; font-size: 3rem; color: #ffb347; animation: float 9s ease-in-out infinite alternate;">🍁</div>

    <!-- Contenido principal -->
    <div class="container">
        <h1>Para Mi Morchis ❤</h1>
        
        <div class="heart-btn-container">
            <button id="heart-btn" class="heart-btn">¡Toca para amor y apoyo!</button>
            <div id="click-counter" class="click-counter">0</div>
        </div>
        
        <div class="message-container">
            <div id="message-box" class="message-box">
                <p id="message-text" class="message-text">Haz clic en el botón para recibir un mensaje especial</p>
            </div>
        </div>
        
        <div class="signature">Te ama Deidei ❤</div>
    </div>

    <audio id="sound-effect" preload="auto">
        <source src="https://assets.mixkit.co/sfx/preview/mixkit-cat-meow-119.mp3" type="audio/mpeg">
    </audio>

    <script>
        // Mensajes de apoyo y amor
        const mensajes = [
            "Eres el mejor novio torpe 🥴💖",
            "Mi bombón 🍫😘",
            "¿A dónde tan guapo? 😏🔥",
            "Tú eres mi mundo 🌎💫",
            "Por esos ojos cansados yo mato 👀💘",
            "En tus malos momentos, cuenta conmigo siempre 🥺💕",
            "Eres mi lugar seguro en este mundo 🌍❤",
            "Juntos podemos con todo lo que venga 💪🌈",
            "Tu sonrisa es mi mayor tesoro 😊💎",
            "Eres más fuerte de lo que crees 💪🌟",
            "No estás solo, siempre estaré aquí contigo 🤝💫",
            "Tu valentía me inspira cada día 🦁✨",
            "Eres mi héroe en buenos y malos momentos 🦸‍♂❤",
            "Tu corazón es tan grande como tu sonrisa 💖😊",
            "En tus días grises, yo seré tu arcoíris 🌈☔",
            "Eres mi persona favorita en el universo entero 🌌💫",
            "Contigo, todo es más bonito y más fácil 🌸✨",
            "Tu bienestar es mi prioridad número uno 🥇❤",
            "Eres increíble tal como eres 💖🌟",
            "Juntos formamos un equipo invencible ⚔🛡"
        ];
        
        // Elementos DOM
        const heartBtn = document.getElementById('heart-btn');
        const messageBox = document.getElementById('message-box');
        const messageText = document.getElementById('message-text');
        const soundEffect = document.getElementById('sound-effect');
        const clickCounter = document.getElementById('click-counter');
        
        // Variables de estado
        let mensajesDisponibles = [...mensajes]; // Copia de todos los mensajes
        let mensajesMostrados = [];
        let clickCount = 0;
        
        // Actualizar contador de clics
        function actualizarContador() {
            clickCounter.textContent = clickCount;
            clickCounter.style.background = clickCount % 2 === 0 ? '#ffcc33' : '#ff6b6b';
        }
        
        // Función para crear corazones flotantes
        function createHearts() {
            const colors = ['#ff6b6b', '#ff8e8e', '#ffb347', '#ffcc33', '#ff7676'];
            const count = 10 + clickCount * 2;
            
            for (let i = 0; i < count; i++) {
                const heart = document.createElement('div');
                heart.className = 'hearts';
                heart.innerHTML = '❤';
                heart.style.left = Math.random() * 100 + 'vw';
                heart.style.fontSize = (Math.random() * 20 + 15) + 'px';
                heart.style.color = colors[Math.floor(Math.random() * colors.length)];
                heart.style.animationDuration = (Math.random() * 3 + 2) + 's';
                heart.style.animationDelay = (Math.random() * 1) + 's';
                document.body.appendChild(heart);
                
                // Eliminar después de la animación
                setTimeout(() => {
                    heart.remove();
                }, 5000);
            }
        }
        
        // Función para mostrar mensaje aleatorio sin repetición
        function showRandomMessage() {
            // Ocultar mensaje actual
            messageBox.classList.remove('show');
            
            setTimeout(() => {
                // Si no quedan mensajes disponibles, resetear
                if (mensajesDisponibles.length === 0) {
                    mensajesDisponibles = [...mensajes];
                    mensajesMostrados = [];
                }
                
                // Seleccionar mensaje aleatorio de los disponibles
                const randomIndex = Math.floor(Math.random() * mensajesDisponibles.length);
                const randomMessage = mensajesDisponibles[randomIndex];
                
                // Mover mensaje de disponibles a mostrados
                mensajesDisponibles.splice(randomIndex, 1);
                mensajesMostrados.push(randomMessage);
                
                // Actualizar texto
                messageText.textContent = randomMessage;
                
                // Mostrar con animación
                messageBox.classList.add('show');
                
                // Reproducir sonido
                soundEffect.currentTime = 0;
                soundEffect.play();
                
                // Crear corazones
                createHearts();
                
                // Incrementar contador
                clickCount++;
                
                // Actualizar contador
                actualizarContador();
                
                // Cambiar color del botón cada 3 clics
                const btnColors = [
                    'linear-gradient(45deg, #ff6b6b, #ff8e8e)',
                    'linear-gradient(45deg, #ffb347, #ffcc33)',
                    'linear-gradient(45deg, #6b5b95, #d64161)',
                    'linear-gradient(45deg, #ff7676, #fdcb6e)',
                    'linear-gradient(45deg, #00b09b, #96c93d)'
                ];
                
                if (clickCount % 3 === 0) {
                    const colorIndex = Math.floor(Math.random() * btnColors.length);
                    heartBtn.style.background = btnColors[colorIndex];
                }
                
                // Efecto especial cada 5 clics
                if (clickCount % 5 === 0) {
                    createSpecialEffect();
                }
            }, 300);
        }
        
        // Función para crear efecto especial
        function createSpecialEffect() {
            const effect = document.createElement('div');
            effect.style.position = 'fixed';
            effect.style.top = '0';
            effect.style.left = '0';
            effect.style.width = '100%';
            effect.style.height = '100%';
            effect.style.background = 'radial-gradient(circle, rgba(255,200,200,0.3) 0%, transparent 70%)';
            effect.style.animation = 'fadeOut 2s forwards';
            effect.style.zIndex = '5';
            effect.style.pointerEvents = 'none';
            
            document.body.appendChild(effect);
            
            // Crear estrellas mágicas
            for (let i = 0; i < 15; i++) {
                setTimeout(() => {
                    const star = document.createElement('div');
                    star.innerHTML = '✨';
                    star.style.position = 'absolute';
                    star.style.left = Math.random() * 100 + 'vw';
                    star.style.top = Math.random() * 100 + 'vh';
                    star.style.fontSize = (Math.random() * 20 + 10) + 'px';
                    star.style.animation = twinkle ${Math.random() * 2 + 1}s infinite alternate;
                    document.body.appendChild(star);
                    
                    setTimeout(() => {
                        star.remove();
                    }, 2000);
                }, i * 100);
            }
            
            // Agregar animación de fadeOut
            const style = document.createElement('style');
            style.innerHTML = `
                @keyframes fadeOut {
                    0% { opacity: 1; }
                    100% { opacity: 0; }
                }
            `;
            document.head.appendChild(style);
            
            setTimeout(() => {
                effect.remove();
                document.head.removeChild(style);
            }, 2000);
        }
        
        // Event listener para el botón
        heartBtn.addEventListener('click', showRandomMessage);
        
        // Mostrar primer mensaje después de un breve retraso
        setTimeout(() => {
            messageBox.classList.add('show');
            actualizarContador();
        }, 1000);
        
        // Crear elementos decorativos adicionales
        function createDecorativeElements() {
            const elements = ['🍄', '🦋', '🍁', '🍂', '🌸', '🌼'];
            
            for (let i = 0; i < 10; i++) {
                const element = document.createElement('div');
                element.className = 'decorative-element';
                element.innerHTML = elements[Math.floor(Math.random() * elements.length)];
                
                // Estilo aleatorio
                const size = Math.random() * 30 + 20;
                const rotation = Math.random() * 30 - 15;
                const color = hsl(${Math.random() * 40 + 20}, 70%, 60%);
                
                element.style.fontSize = size + 'px';
                element.style.color = color;
                element.style.transform = rotate(${rotation}deg);
                element.style.left = Math.random() * 90 + 5 + '%';
                element.style.top = Math.random() * 90 + 5 + '%';
                element.style.animationDuration = (Math.random() * 5 + 5) + 's';
                
                document.body.appendChild(element);
            }
        }
        
        // Inicializar
        window.onload = function() {
            createDecorativeElements();
        };
    </script>
</body>
</html>
