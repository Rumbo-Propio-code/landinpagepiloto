<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Rumbo Propio — Valida tu emprendimiento antes de comprometer tus ahorros.">
    <title>Rumbo Propio — Agenda tu sesión gratuita</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=Montserrat:wght@700;800;900&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --navy: #1B3B5A;      /* Azul del logo */
            --terracotta: #B55D32; /* Cobre del logo */
            --navy-dark: #12283D;
            --white: #FFFFFF;
            --gray-light: #F4F7F9;
            --text-main: #2D3748;
            --text-muted: #718096;
            --sans: 'Inter', sans-serif;
            --titles: 'Montserrat', sans-serif;
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }
        html { scroll-behavior: smooth; }
        body { 
            font-family: var(--sans); 
            color: var(--text-main); 
            line-height: 1.6; 
            background-color: var(--white);
            -webkit-font-smoothing: antialiased;
        }

        /* --- NAVEGACIÓN --- */
        nav {
            position: fixed; top: 0; width: 100%; height: 70px;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(8px);
            border-bottom: 1px solid #E2E8F0;
            display: flex; align-items: center; justify-content: space-between;
            padding: 0 5%; z-index: 1000;
        }
        .nav-brand {
            font-family: var(--titles); font-weight: 800;
            color: var(--navy); font-size: 1.2rem;
            display: flex; align-items: center; gap: 8px;
            text-transform: uppercase; letter-spacing: 1px;
        }
        .nav-btn {
            background: var(--terracotta); color: white;
            padding: 10px 20px; border-radius: 4px;
            text-decoration: none; font-weight: 600; font-size: 0.9rem;
            transition: 0.3s;
        }
        .nav-btn:hover { background: var(--navy); }

        /* --- HERO --- */
        .hero {
            padding: 140px 5% 80px;
            background: linear-gradient(135deg, var(--white) 0%, var(--gray-light) 100%);
            text-align: center;
        }
        .hero-tag {
            color: var(--terracotta); font-weight: 600; font-size: 0.85rem;
            text-transform: uppercase; letter-spacing: 2px; margin-bottom: 20px;
        }
        .hero h1 {
            font-family: var(--titles); font-size: clamp(2.2rem, 8vw, 3.8rem);
            color: var(--navy); line-height: 1.1; margin-bottom: 24px;
        }
        .hero p {
            max-width: 650px; margin: 0 auto 40px; font-size: 1.15rem; color: var(--text-muted);
        }
        .btn-main {
            display: inline-block; background: var(--terracotta); color: white;
            padding: 20px 40px; border-radius: 4px; font-weight: 700;
            text-decoration: none; font-size: 1.1rem; transition: 0.3s;
            box-shadow: 0 4px 15px rgba(181, 93, 50, 0.3);
        }
        .btn-main:hover { transform: translateY(-2px); box-shadow: 0 6px 20px rgba(181, 93, 50, 0.4); }

        /* --- MÉTRICAS --- */
        .stats {
            display: grid; grid-template-columns: repeat(2, 1fr);
            gap: 15px; max-width: 900px; margin: -40px auto 0;
            padding: 0 5%;
        }
        .stat-card {
            background: var(--navy); color: white; padding: 25px;
            border-radius: 8px; text-align: center;
        }
        .stat-val { font-family: var(--titles); font-size: 1.8rem; display: block; color: var(--terracotta); }
        .stat-lbl { font-size: 0.8rem; text-transform: uppercase; opacity: 0.8; }

        /* --- SECCIONES --- */
        section { padding: 100px 5%; }
        .section-title { text-align: center; margin-bottom: 60px; }
        .section-title h2 { font-family: var(--titles); font-size: 2.2rem; color: var(--navy); margin-bottom: 15px; }
        .section-title p { color: var(--text-muted); max-width: 600px; margin: 0 auto; }

        /* --- ETAPAS --- */
        .etapas { display: grid; gap: 20px; }
        .etapa {
            border-left: 4px solid var(--terracotta);
            background: var(--gray-light); padding: 30px; border-radius: 0 8px 8px 0;
        }
        .etapa-num { color: var(--terracotta); font-weight: 800; font-size: 1.2rem; margin-bottom: 10px; display: block; }
        .etapa h3 { font-family: var(--titles); color: var(--navy); margin-bottom: 10px; }

        /* --- AGENDAR (CAL.COM) --- */
        .booking-section { background: var(--navy-dark); color: white; border-radius: 12px; margin: 0 5% 100px; padding: 60px 20px; text-align: center; }
        .calendar-wrapper { 
            max-width: 850px; margin: 40px auto 0; 
            background: white; border-radius: 8px; overflow: hidden;
            box-shadow: 0 20px 40px rgba(0,0,0,0.2);
        }

        @media (min-width: 768px) {
            .stats { grid-template-columns: repeat(4, 1fr); }
            .etapas { grid-template-columns: repeat(3, 1fr); }
            .hero { padding: 180px 5% 120px; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="nav-brand">Rumbo Propio</div>
        <a href="#agendar" class="nav-btn">Agenda gratis</a>
    </nav>

    <header class="hero">
        <div class="hero-tag">Profesionales Senior · Chile 2026</div>
        <h1>¿Emprender o<br>equivocarte?</h1>
        <p>Valida si tu idea tiene mercado real antes de comprometer tus ahorros. Un método probado para convertir tu experiencia en un activo propio.</p>
        <a href="#agendar" class="btn-main">Agendar Diagnóstico Sin Costo →</a>
    </header>

    <div class="stats">
        <div class="stat-card"><span class="stat-val">11</span><span class="stat-lbl">Sesiones 1:1</span></div>
        <div class="stat-card"><span class="stat-val">3-5</span><span class="stat-lbl">Ventas Reales</span></div>
        <div class="stat-card"><span class="stat-val">12M</span><span class="stat-lbl">Hoja de Ruta</span></div>
        <div class="stat-card"><span class="stat-val">48 UF</span><span class="stat-lbl">Inversión Total</span></div>
    </div>

    <section id="programa">
        <div class="section-title">
            <h2>El veredicto que necesitas</h2>
            <p>Un acompañamiento técnico que separa la validación del riesgo financiero.</p>
        </div>
        <div class="etapas">
            <div class="etapa">
                <span class="etapa-num">01</span>
                <h3>Diagnóstico</h3>
                <p>Análisis de perfil, mercado y veredicto de viabilidad en la sesión 4.</p>
            </div>
            <div class="etapa">
                <span class="etapa-num">02</span>
                <h3>Prueba Piloto</h3>
                <p>Modelo de negocio, lanzamiento y cierre de las primeras ventas reales.</p>
            </div>
            <div class="etapa">
                <span class="etapa-num">03</span>
                <h3>Planeamiento</h3>
                <p>Proyección a 12 meses y rutina diaria para una gestión autónoma.</p>
            </div>
        </div>
    </section>

    <div id="agendar" class="booking-section">
        <h2 style="font-family: var(--titles); font-size: 2.2rem; margin-bottom: 10px;">Elige tu horario</h2>
        <p style="opacity: 0.8; max-width: 500px; margin: 0 auto;">Sesión inicial de 30 minutos. Sin costo. Sin compromiso. Confirmación inmediata.</p>
        
        <div class="calendar-wrapper">
            <iframe 
                src="https://cal.com/rumbo-propio?embed=true" 
                style="width:100%; height:650px; border:none;" 
                loading="lazy">
            </iframe>
        </div>
        
        <p style="margin-top: 30px; font-size: 0.9rem;">
            ¿Problemas con el calendario? 
            <a href="https://cal.com/rumbo-propio" target="_blank" style="color: var(--terracotta); font-weight: 600;">Abrir enlace directo</a>
        </p>
    </div>

    <footer style="padding: 40px 5%; background: var(--gray-light); text-align: center; font-size: 0.85rem; color: var(--text-muted); border-top: 1px solid #E2E8F0;">
        <p>© 2026 Rumbo Propio · Asesoría para Profesionales Senior · Chile</p>
    </footer>

</body>
</html>
