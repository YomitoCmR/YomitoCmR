<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>YomitoCmR | Official Site 🔥</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;900&family=Oswald:wght@300;700&display=swap');

        :root {
            --fire: #ff4500;
            --smoke: #1a1a1a;
            --dark: #050505;
        }

        body {
            margin: 0;
            background-color: var(--dark);
            color: white;
            font-family: 'Oswald', sans-serif;
            overflow-x: hidden;
        }

        /* --- EFECTO FUEGO --- */
        .fire-text {
            font-family: 'Orbitron', sans-serif;
            color: #fff;
            text-shadow: 0 0 10px #fff, 0 0 20px var(--fire), 0 0 40px var(--fire);
            animation: flicker 1.5s infinite alternate;
        }

        @keyframes flicker {
            0% { opacity: 0.9; text-shadow: 0 0 10px var(--fire); }
            100% { opacity: 1; text-shadow: 0 0 25px var(--fire), 0 0 50px #ff0000; }
        }

        /* --- HERO --- */
        .hero {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background: linear-gradient(to bottom, rgba(0,0,0,0.5), var(--dark)),
                        url('https://images.unsplash.com/photo-1516450360452-9312f5e86fc7?q=80&w=2070&auto=format&fit=crop'); /* Imagen de fondo estilo concierto */
            background-size: cover;
            background-position: center;
        }

        .hero h1 { font-size: 5rem; margin: 0; text-transform: uppercase; }

        /* --- MÚSICA & CARDS --- */
        .section { padding: 100px 20px; text-align: center; }
        
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            max-width: 1200px;
            margin: 50px auto;
        }

        .card {
            background: var(--smoke);
            border-radius: 15px;
            padding: 20px;
            transition: transform 0.3s ease;
            border: 1px solid #333;
        }

        .card:hover {
            transform: translateY(-10px);
            border-color: var(--fire);
        }

        .card img { width: 100%; border-radius: 10px; margin-bottom: 15px; }

        /* --- FORMULARIO DE CONTACTO --- */
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background: #111;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(255, 69, 0, 0.2);
        }

        input, textarea {
            width: 100%;
            padding: 15px;
            margin-bottom: 20px;
            background: #222;
            border: 1px solid #444;
            color: white;
            border-radius: 5px;
        }

        .btn-fire {
            background: var(--fire);
            color: white;
            border: none;
            padding: 15px 40px;
            font-weight: bold;
            cursor: pointer;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .btn-fire:hover { background: #e63e00; }

    </style>
</head>
<body>

    <section class="hero">
        <h1 class="fire-text">YomitoCmR</h1>
        <p style="letter-spacing: 5px; font-size: 1.2rem;">RISING STAR | REBIRTH</p>
    </section>

    <section id="music" class="section">
        <h2 style="font-size: 3rem;">LATEST HITS 🔥</h2>
        <div class="grid">
            <div class="card">
                <img src="https://via.placeholder.com/400x400/1a1a1a/ff4500?text=Rising+Star" alt="Rising Star">
                <h3>Rising Star</h3>
                <p>EP Completo</p>
                <button class="btn-fire">ESCUCHAR</button>
            </div>
            <div class="card">
                <img src="https://via.placeholder.com/400x400/1a1a1a/ff4500?text=uuyMaMa" alt="uuyMaMa">
                <h3>uuyMaMa</h3>
                <p>Single</p>
                <button class="btn-fire">ESCUCHAR</button>
            </div>
            <div class="card">
                <img src="https://via.placeholder.com/400x400/1a1a1a/ff4500?text=De+ahora+pa,+ahora" alt="De ahora pa ahora">
                <h3>De ahora pa, ahora</h3>
                <p>Próximamente</p>
                <button class="btn-fire">PRE-SAVE</button>
            </div>
        </div>
    </section>

    <section id="contact" class="section">
        <h2>CONTACTO & BOOKING</h2>
        <div class="contact-form">
            <form>
                <input type="text" placeholder="Tu Nombre / Promotora" required>
                <input type="email" placeholder="Correo Electrónico" required>
                <textarea rows="5" placeholder="Cuéntame sobre tu evento o propuesta..."></textarea>
                <button type="submit" class="btn-fire">ENVIAR MENSAJE</button>
            </form>
        </div>
    </section>

    <footer style="padding: 50px; text-align: center; border-top: 1px solid #222;">
        <p>YomitoCmR &copy; 2026 | El fuego nunca se apaga.</p>
    </footer>

</body>
</html>
