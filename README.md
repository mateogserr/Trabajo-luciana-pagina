<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Clínica Ginecológica y Obstétrica | Dra. Luciana Martínez Pacheco</title>
  <meta name="description" content="Clínica ginecológica y obstétrica con atención especializada, agenda de citas, consultas virtuales, videos, biblioteca PDF y equipo profesional." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">
  <style>
    :root{
      --bg:#f5f8fc;
      --card:#ffffff;
      --text:#183153;
      --muted:#5f6f87;
      --primary:#0b74de;
      --primary-2:#00a3ff;
      --accent:#12b886;
      --line:#e7edf5;
      --shadow:0 16px 40px rgba(16, 38, 71, .10);
      --radius:22px;
    }

    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0;
      font-family:"Inter",system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;
      background:
        radial-gradient(circle at top left, rgba(11,116,222,.08), transparent 28%),
        radial-gradient(circle at top right, rgba(18,184,134,.08), transparent 24%),
        var(--bg);
      color:var(--text);
    }

    a{color:inherit}
    .wrap{width:min(1180px, calc(100% - 32px)); margin:0 auto}

    .topbar{
      background:#08305c;
      color:#dbe9ff;
      font-size:.92rem;
      padding:10px 0;
    }
    .topbar .wrap{
      display:flex;
      gap:12px;
      justify-content:space-between;
      align-items:center;
      flex-wrap:wrap;
    }

    header.hero{
      position:relative;
      overflow:hidden;
      padding:42px 0 28px;
    }
    .hero-card{
      background:linear-gradient(135deg, #0b74de 0%, #0f5bbd 48%, #0aa3d9 100%);
      color:#fff;
      border-radius:34px;
      box-shadow:var(--shadow);
      padding:34px;
      position:relative;
    }
    .hero-grid{
      display:grid;
      grid-template-columns:1.5fr 1fr;
      gap:28px;
      align-items:center;
    }
    .eyebrow{
      display:inline-flex;
      align-items:center;
      gap:10px;
      font-weight:700;
      letter-spacing:.02em;
      text-transform:uppercase;
      font-size:.8rem;
      background:rgba(255,255,255,.14);
      border:1px solid rgba(255,255,255,.18);
      padding:10px 14px;
      border-radius:999px;
      margin-bottom:16px;
    }
    .hero h1{
      margin:0 0 14px;
      font-size:clamp(2rem, 4vw, 3.6rem);
      line-height:1.06;
    }
    .hero p{
      margin:0 0 22px;
      max-width:62ch;
      color:rgba(255,255,255,.92);
      font-size:1.05rem;
      line-height:1.7;
    }
    .hero-actions{
      display:flex;
      gap:12px;
      flex-wrap:wrap;
      margin-top:18px;
    }
    .btn{
      display:inline-flex;
      align-items:center;
      gap:10px;
      text-decoration:none;
      border:none;
      cursor:pointer;
      padding:13px 18px;
      border-radius:16px;
      font-weight:700;
      transition:.2s transform ease, .2s opacity ease, .2s background ease;
    }
    .btn:hover{transform:translateY(-1px)}
    .btn-primary{background:#fff;color:#0b74de}
    .btn-ghost{background:rgba(255,255,255,.14); color:#fff; border:1px solid rgba(255,255,255,.18)}

    .hero-side{
      background:rgba(255,255,255,.12);
      border:1px solid rgba(255,255,255,.18);
      border-radius:28px;
      padding:22px;
      backdrop-filter: blur(8px);
    }
    .mini-stats{
      display:grid;
      gap:12px;
    }
    .stat{
      background:rgba(255,255,255,.12);
      border:1px solid rgba(255,255,255,.14);
      border-radius:18px;
      padding:14px 16px;
    }
    .stat strong{display:block; font-size:1.05rem; margin-bottom:3px}
    .stat span{color:rgba(255,255,255,.84); font-size:.94rem}

    nav{
      position:sticky;
      top:0;
      z-index:1000;
      background:rgba(255,255,255,.86);
      backdrop-filter: blur(10px);
      border-bottom:1px solid rgba(231,237,245,.85);
    }
    .nav-inner{
      display:flex;
      gap:10px;
      flex-wrap:wrap;
      justify-content:center;
      padding:12px 0;
    }
    .nav-inner a{
      text-decoration:none;
      color:var(--text);
      font-weight:700;
      font-size:.95rem;
      padding:10px 14px;
      border-radius:999px;
    }
    .nav-inner a:hover{background:#eaf3ff;color:#0b74de}

    main{padding:28px 0 56px}
    section{margin:0 0 24px}
    .section-title{
      display:flex;
      align-items:end;
      justify-content:space-between;
      gap:16px;
      margin:0 0 14px;
      flex-wrap:wrap;
    }
    .section-title h2{
      margin:0;
      font-size:1.55rem;
    }
    .section-title p{
      margin:0;
      color:var(--muted);
      max-width:75ch;
      line-height:1.6;
    }

    .card{
      background:var(--card);
      border:1px solid rgba(231,237,245,.95);
      border-radius:var(--radius);
      box-shadow:var(--shadow);
      padding:24px;
    }

    .grid-2{display:grid; grid-template-columns:1.15fr .85fr; gap:22px}
    .grid-3{display:grid; grid-template-columns:repeat(3,1fr); gap:18px}
    .grid-4{display:grid; grid-template-columns:repeat(4,1fr); gap:18px}
    .soft{
      background:linear-gradient(180deg, #ffffff, #f8fbff);
      border:1px solid var(--line);
      border-radius:18px;
      padding:18px;
    }
    .pill{
      display:inline-flex;
      align-items:center;
      gap:8px;
      padding:8px 12px;
      border-radius:999px;
      background:#eef6ff;
      color:#0b74de;
      font-size:.9rem;
      font-weight:700;
      margin:4px 8px 0 0;
    }

    .map{
      width:100%;
      border:0;
      height:340px;
      border-radius:18px;
      overflow:hidden;
    }

    .services{
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(220px, 1fr));
      gap:16px;
    }
    .service{
      padding:18px;
      border-radius:18px;
      border:1px solid var(--line);
      background:linear-gradient(180deg, #ffffff, #f7fbff);
      min-height:128px;
    }
    .service i{font-size:1.25rem; color:var(--primary); margin-bottom:12px}
    .service h3{margin:0 0 8px; font-size:1.02rem}
    .service p{margin:0; color:var(--muted); line-height:1.55; font-size:.95rem}

    .people{
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(250px, 1fr));
      gap:16px;
    }
    .person{
      border:1px solid var(--line);
      border-radius:20px;
      overflow:hidden;
      background:#fff;
    }
    .person .cover{
      height:92px;
      background:linear-gradient(135deg, rgba(11,116,222,.22), rgba(18,184,134,.18));
    }
    .person .body{padding:16px}
    .avatar{
      width:64px;height:64px;border-radius:18px;
      margin-top:-44px;
      background:#0b74de;
      color:#fff;
      display:grid;place-items:center;
      font-weight:800;
      box-shadow:0 10px 24px rgba(11,116,222,.24);
    }
    .person h3{margin:12px 0 6px}
    .person .role{color:var(--primary); font-weight:700; font-size:.92rem}
    .person p{color:var(--muted); line-height:1.6; margin:10px 0 0; font-size:.95rem}

    .timeline{
      border-left:3px solid #dbe7f5;
      margin:18px 0 0 10px;
      padding-left:18px;
      display:grid;
      gap:16px;
    }
    .timeline-item{
      position:relative;
      padding:14px 16px;
      border-radius:16px;
      background:#fbfdff;
      border:1px solid var(--line);
    }
    .timeline-item::before{
      content:"";
      position:absolute;
      left:-27px;
      top:18px;
      width:12px;height:12px;border-radius:50%;
      background:var(--primary);
      border:3px solid #fff;
      box-shadow:0 0 0 2px #dbe7f5;
    }
    .timeline-item h4{margin:0 0 6px}
    .timeline-item span{color:var(--muted); font-size:.93rem}
    .timeline-item p{margin:10px 0 0; color:var(--muted); line-height:1.6}

    .video-grid{
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(300px, 1fr));
      gap:16px;
    }
    .video{
      border-radius:18px;
      overflow:hidden;
      border:1px solid var(--line);
      background:#000;
    }
    .video iframe{
      width:100%;
      aspect-ratio:16/9;
      border:0;
      display:block;
    }
    .video .caption{
      padding:14px 16px;
      background:#fff;
      color:var(--muted);
      font-size:.95rem;
      line-height:1.55;
    }

    .pdf-list{
      display:grid;
      gap:14px;
    }
    .pdf-item{
      display:flex;
      justify-content:space-between;
      gap:14px;
      align-items:center;
      padding:16px 18px;
      border:1px solid var(--line);
      border-radius:16px;
      background:#fff;
      flex-wrap:wrap;
    }
    .pdf-item strong{display:block; margin-bottom:4px}
    .pdf-item span{color:var(--muted); font-size:.94rem}
    .pdf-item a{
      text-decoration:none;
      background:#eaf4ff;
      color:#0b74de;
      padding:10px 14px;
      border-radius:12px;
      font-weight:700;
      white-space:nowrap;
    }

    .schedule-wrap{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:18px;
      align-items:start;
    }
    .calendar{
      border:1px solid var(--line);
      border-radius:20px;
      background:#fff;
      overflow:hidden;
    }
    .cal-head{
      display:flex;
      justify-content:space-between;
      align-items:center;
      gap:10px;
      padding:16px 18px;
      background:linear-gradient(135deg, #0b74de, #0aa3d9);
      color:#fff;
    }
    .cal-head button{
      border:none; cursor:pointer;
      background:rgba(255,255,255,.14);
      color:#fff;
      width:38px;height:38px;border-radius:12px;
      font-size:1rem;
    }
    .cal-grid{
      display:grid;
      grid-template-columns:repeat(7, 1fr);
      gap:8px;
      padding:14px;
    }
    .dow{
      text-align:center;
      font-size:.83rem;
      color:var(--muted);
      font-weight:700;
      padding:4px 0;
    }
    .day{
      min-height:72px;
      border-radius:14px;
      border:1px solid var(--line);
      padding:8px;
      background:#fbfdff;
      display:flex;
      flex-direction:column;
      justify-content:space-between;
      cursor:pointer;
      transition:.15s transform ease, .15s box-shadow ease;
    }
    .day:hover{transform:translateY(-1px); box-shadow:0 10px 22px rgba(16,38,71,.08)}
    .day.muted{opacity:.38; cursor:default}
    .day strong{font-size:.95rem}
    .day small{font-size:.76rem; color:var(--muted)}
    .day.selected{
      border-color:#0b74de;
      box-shadow:0 0 0 3px rgba(11,116,222,.12);
      background:#eef6ff;
    }
    .dot{
      width:8px;height:8px;border-radius:50%;
      background:var(--accent);
      display:inline-block;
    }

    label{display:block; font-weight:700; margin:12px 0 7px}
    input, select, textarea{
      width:100%;
      padding:13px 14px;
      border-radius:14px;
      border:1px solid #d8e2ee;
      background:#fff;
      color:var(--text);
      font:inherit;
      outline:none;
    }
    input:focus, select:focus, textarea:focus{
      border-color:#0b74de;
      box-shadow:0 0 0 4px rgba(11,116,222,.08);
    }
    textarea{min-height:116px; resize:vertical}
    .form-actions{
      display:flex;
      gap:10px;
      flex-wrap:wrap;
      margin-top:14px;
    }

    .appointment-list{
      display:grid;
      gap:12px;
      margin-top:16px;
    }
    .appointment{
      border:1px solid var(--line);
      border-radius:16px;
      background:#fbfdff;
      padding:14px 16px;
    }
    .appointment strong{display:block; margin-bottom:4px}
    .appointment span{color:var(--muted); font-size:.94rem; line-height:1.5}

    .social{
      display:flex;
      flex-wrap:wrap;
      gap:12px;
    }
    .social a{
      text-decoration:none;
      background:#fff;
      border:1px solid var(--line);
      width:52px;height:52px;
      border-radius:16px;
      display:grid;
      place-items:center;
      font-size:1.2rem;
      color:#0b74de;
      box-shadow:0 10px 24px rgba(16,38,71,.06);
    }

    .notice{
      border-left:4px solid var(--accent);
      background:#f0fff8;
      color:#1d5f4d;
      padding:14px 16px;
      border-radius:14px;
      line-height:1.6;
      margin-top:14px;
    }

    .footer{
      margin-top:18px;
      padding:24px 0 34px;
      color:var(--muted);
      text-align:center;
    }

    .floating{
      position:fixed;
      right:18px;
      bottom:18px;
      display:grid;
      gap:10px;
      z-index:1200;
    }
    .floating a{
      width:54px;height:54px;border-radius:18px;
      display:grid;place-items:center;
      color:#fff;
      box-shadow:var(--shadow);
      text-decoration:none;
      font-size:1.2rem;
    }
    .wa{background:#25D366}
    .mapbtn{background:#0b74de}

    @media (max-width: 980px){
      .hero-grid,.grid-2,.schedule-wrap{grid-template-columns:1fr}
      .grid-3,.grid-4{grid-template-columns:1fr 1fr}
    }
    @media (max-width: 640px){
      .wrap{width:min(100% - 20px, 1180px)}
      .hero-card{padding:24px}
      .card{padding:18px}
      .grid-3,.grid-4{grid-template-columns:1fr}
      .cal-grid{gap:6px; padding:10px}
      .day{min-height:64px}
      .nav-inner a{padding:9px 12px}
    }
  </style>
</head>
<body>

  <div class="topbar">
    <div class="wrap">
      <div><i class="fa-solid fa-location-dot"></i> Calle Beni Nº 377</div>
      <div><i class="fa-solid fa-phone"></i> 62503587</div>
      <div><i class="fa-solid fa-user-doctor"></i> Dra. Luciana Martínez Pacheco</div>
    </div>
  </div>

  <header class="hero">
    <div class="wrap">
      <div class="hero-card">
        <div class="hero-grid">
          <div>
            <div class="eyebrow"><i class="fa-solid fa-heart-pulse"></i> Salud femenina integral</div>
            <h1>Clínica Ginecológica y Obstétrica</h1>
            <p>
              Atención especializada en ginecología, obstetricia, control prenatal, seguimiento de embarazo,
              prevención, educación y consulta virtual. Diseño profesional listo para presentar y compartir.
            </p>
            <div class="hero-actions">
              <a class="btn btn-primary" href="#citas"><i class="fa-solid fa-calendar-check"></i> Agendar cita</a>
              <a class="btn btn-ghost" href="#contacto"><i class="fa-solid fa-address-book"></i> Ver contacto</a>
              <a class="btn btn-ghost" href="#virtual"><i class="fa-solid fa-video"></i> Consulta virtual</a>
            </div>
          </div>

          <aside class="hero-side">
            <div class="mini-stats">
              <div class="stat">
                <strong>Ubicación visible</strong>
                <span>Calle Beni Nº 377, acceso rápido desde la página.</span>
              </div>
              <div class="stat">
                <strong>Servicios principales</strong>
                <span>Ginecología, obstetricia, procedimientos, control y prevención.</span>
              </div>
              <div class="stat">
                <strong>Agenda y consulta</strong>
                <span>Calendario interactivo y formulario de consulta virtual.</span>
              </div>
            </div>
          </aside>
        </div>
      </div>
    </div>
  </header>

  <nav>
    <div class="wrap nav-inner">
      <a href="#ubicacion">Ubicación</a>
      <a href="#servicios">Servicios</a>
      <a href="#equipo">Recursos humanos</a>
      <a href="#curriculum">Currículum</a>
      <a href="#videos">Videos</a>
      <a href="#biblioteca">PDF</a>
      <a href="#citas">Citas</a>
      <a href="#virtual">Consultas virtuales</a>
      <a href="#contacto">Contacto</a>
    </div>
  </nav>

  <main class="wrap">
    <section id="ubicacion">
      <div class="section-title">
        <h2>Ubicación de la clínica</h2>
        <p>Mapa integrado para que la dirección sea visible desde la página principal.</p>
      </div>
      <div class="card grid-2">
        <div>
          <span class="pill"><i class="fa-solid fa-location-dot"></i> Calle Beni Nº 377</span>
          <span class="pill"><i class="fa-solid fa-building"></i> Clínica ginecológica y obstétrica</span>
          <div class="notice">
            Dirección de referencia: <strong>Calle Beni Nº 377</strong>. Aquí puedes cambiar el mapa por la ubicación exacta cuando tengas el enlace de Google Maps definitivo.
          </div>
          <div style="margin-top:16px">
            <a class="btn btn-primary" href="https://www.google.com/maps?q=Calle+Beni+377" target="_blank" rel="noopener">
              <i class="fa-solid fa-arrow-up-right-from-square"></i> Abrir en Google Maps
            </a>
          </div>
        </div>
        <div>
          <iframe
            class="map"
            src="https://www.google.com/maps?q=Calle+Beni+377&output=embed"
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
            title="Mapa de ubicación">
          </iframe>
        </div>
      </div>
    </section>

    <section id="servicios">
      <div class="section-title">
        <h2>Servicios ginecológicos y obstétricos</h2>
        <p>Una presentación más completa para mostrar atención, procedimientos y prevención.</p>
      </div>
      <div class="card">
        <div class="services">
          <div class="service">
            <i class="fa-solid fa-person-pregnant"></i>
            <h3>Control prenatal</h3>
            <p>Seguimiento integral del embarazo, evaluación materna y control del bienestar fetal.</p>
          </div>
          <div class="service">
            <i class="fa-solid fa-clipboard-check"></i>
            <h3>Control ginecológico</h3>
            <p>Revisiones periódicas para la prevención, diagnóstico temprano y acompañamiento clínico.</p>
          </div>
          <div class="service">
            <i class="fa-solid fa-microscope"></i>
            <h3>Papanicolaou y colposcopía</h3>
            <p>Detección preventiva y estudio de lesiones cervicales con orientación médica profesional.</p>
          </div>
          <div class="service">
            <i class="fa-solid fa-venus"></i>
            <h3>Planificación familiar</h3>
            <p>Consejería sobre métodos anticonceptivos y salud reproductiva.</p>
          </div>
          <div class="service">
            <i class="fa-solid fa-heart-pulse"></i>
            <h3>Atención obstétrica</h3>
            <p>Seguimiento de embarazo normal y embarazo de mayor riesgo.</p>
          </div>
          <div class="service">
            <i class="fa-solid fa-baby"></i>
            <h3>Ecografía obstétrica</h3>
            <p>Control de desarrollo fetal y apoyo diagnóstico para la toma de decisiones.</p>
          </div>
          <div class="service">
            <i class="fa-solid fa-shield-heart"></i>
            <h3>Prevención y educación</h3>
            <p>Promoción de hábitos saludables y educación en salud femenina.</p>
          </div>
          <div class="service">
            <i class="fa-solid fa-notes-medical"></i>
            <h3>Procedimientos ginecológicos</h3>
            <p>Orientación y acompañamiento en procedimientos diagnósticos y terapéuticos.</p>
          </div>
        </div>
      </div>
    </section>

    <section id="equipo">
      <div class="section-title">
        <h2>Recursos humanos</h2>
        <p>Incluye personal con nombres ficticios para una presentación limpia y profesional.</p>
      </div>
      <div class="card">
        <div class="people">
          <article class="person">
            <div class="cover"></div>
            <div class="body">
              <div class="avatar">LM</div>
              <h3>Dra. Luciana Martínez Pacheco</h3>
              <div class="role">Ginecología y Obstetricia</div>
              <p>Médica responsable del servicio, con atención integral en salud femenina, embarazo y procedimientos ginecológicos.</p>
            </div>
          </article>

          <article class="person">
            <div class="cover"></div>
            <div class="body">
              <div class="avatar">AM</div>
              <h3>Lic. Ana Morales</h3>
              <div class="role">Obstetra</div>
              <p>Apoyo en control prenatal, educación materna y acompañamiento durante consultas.</p>
            </div>
          </article>

          <article class="person">
            <div class="cover"></div>
            <div class="body">
              <div class="avatar">SR</div>
              <h3>Lic. Sofía Rojas</h3>
              <div class="role">Enfermería</div>
              <p>Asistencia clínica, toma de signos vitales, preparación de pacientes y seguimiento.</p>
            </div>
          </article>

          <article class="person">
            <div class="cover"></div>
            <div class="body">
              <div class="avatar">JP</div>
              <h3>Lic. Juan Pérez</h3>
              <div class="role">Administración</div>
              <p>Gestión de agenda, recepción, organización de citas y atención inicial al paciente.</p>
            </div>
          </article>
        </div>
      </div>
    </section>

    <section id="curriculum">
      <div class="section-title">
        <h2>Currículum profesional</h2>
        <p>Formato tipo ficha profesional para mostrar experiencia, formación y áreas de trabajo.</p>
      </div>
      <div class="card grid-2">
        <div class="soft">
          <h3 style="margin-top:0">Perfil profesional</h3>
          <p style="color:var(--muted); line-height:1.75; margin-bottom:14px">
            La Dra. Luciana Martínez Pacheco brinda atención médica enfocada en la salud integral de la mujer,
            con énfasis en ginecología, obstetricia, prevención, seguimiento prenatal y procedimientos clínicos.
          </p>
          <div>
            <span class="pill">Médico Cirujano</span>
            <span class="pill">Especialidad en Ginecología</span>
            <span class="pill">Especialidad en Obstetricia</span>
            <span class="pill">Control prenatal</span>
            <span class="pill">Salud reproductiva</span>
          </div>
        </div>
        <div class="soft">
          <h3 style="margin-top:0">Experiencia resumida</h3>
          <div class="timeline">
            <div class="timeline-item">
              <h4>Formación médica</h4>
              <span>Base clínica y quirúrgica en salud de la mujer.</span>
              <p>Preparación profesional orientada al diagnóstico y tratamiento de patologías ginecológicas.</p>
            </div>
            <div class="timeline-item">
              <h4>Atención obstétrica</h4>
              <span>Seguimiento de embarazo y control materno-fetal.</span>
              <p>Valoración periódica, prevención de complicaciones y educación para la maternidad segura.</p>
            </div>
            <div class="timeline-item">
              <h4>Procedimientos y prevención</h4>
              <span>Uso de técnicas diagnósticas y educación sanitaria.</span>
              <p>Incluye ecografía, tamizaje, revisión clínica y orientación preventiva.</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="videos">
      <div class="section-title">
        <h2>Videos educativos</h2>
        <p>Dos videos integrados para mostrarse directamente en la misma página. Puedes reemplazar los enlaces por los de tu preferencia.</p>
      </div>
      <div class="card">
        <div class="video-grid">
          <div class="video">
            <iframe
              src="https://www.youtube-nocookie.com/embed/0Vd8z1Yl7VQ"
              title="Video educativo sobre procedimiento ginecológico"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
              allowfullscreen></iframe>
            <div class="caption">Video 1: contenido educativo sobre procedimientos ginecológicos.</div>
          </div>
          <div class="video">
            <iframe
              src="https://www.youtube-nocookie.com/embed/5Jm2f1R4w7A"
              title="Video educativo sobre procedimiento obstétrico"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
              allowfullscreen></iframe>
            <div class="caption">Video 2: contenido educativo sobre procedimientos obstétricos.</div>
          </div>
        </div>
      </div>
    </section>

    <section id="biblioteca">
      <div class="section-title">
        <h2>Artículos PDF anclados</h2>
        <p>Enlaces listos para conectar con documentos PDF de la clínica o material científico.</p>
      </div>
      <div class="card">
        <div class="pdf-list">
          <div class="pdf-item">
            <div>
              <strong>Guía de control prenatal</strong>
              <span>Material informativo para pacientes y estudiantes.</span>
            </div>
            <a href="documentos/guia-control-prenatal.pdf" target="_blank" rel="noopener">
              <i class="fa-solid fa-file-pdf"></i> Ver PDF
            </a>
          </div>
          <div class="pdf-item">
            <div>
              <strong>Prevención y diagnóstico temprano del cáncer cervicouterino</strong>
              <span>Artículo orientado a prevención, tamizaje y educación.</span>
            </div>
            <a href="documentos/cancer-cervicouterino.pdf" target="_blank" rel="noopener">
              <i class="fa-solid fa-file-pdf"></i> Ver PDF
            </a>
          </div>
        </div>
      </div>
    </section>

    <section id="citas">
      <div class="section-title">
        <h2>Calendario para agendamiento de citas</h2>
        <p>Agenda visual con selección de fecha y formulario. Guarda las citas en el navegador para mostrar una experiencia más real.</p>
      </div>
      <div class="card">
        <div class="schedule-wrap">
          <div class="calendar">
            <div class="cal-head">
              <button type="button" id="prevMonth" aria-label="Mes anterior"><i class="fa-solid fa-chevron-left"></i></button>
              <div>
                <strong id="monthLabel" style="display:block;font-size:1.05rem"></strong>
                <small id="todayLabel" style="opacity:.9"></small>
              </div>
              <button type="button" id="nextMonth" aria-label="Mes siguiente"><i class="fa-solid fa-chevron-right"></i></button>
            </div>
            <div class="cal-grid" id="dow"></div>
            <div class="cal-grid" id="calendarGrid"></div>
          </div>

          <div class="soft">
            <h3 style="margin-top:0">Solicitar cita</h3>
            <form id="appointmentForm">
              <label for="name">Nombre completo</label>
              <input id="name" type="text" placeholder="Escribe tu nombre" required>

              <label for="phone">Teléfono</label>
              <input id="phone" type="tel" placeholder="Ej. 62503587" required>

              <label for="date">Fecha elegida</label>
              <input id="date" type="text" placeholder="Selecciona una fecha en el calendario" readonly required>

              <label for="time">Hora</label>
              <input id="time" type="time" required>

              <label for="reason">Motivo de consulta</label>
              <textarea id="reason" placeholder="Describe brevemente el motivo"></textarea>

              <div class="form-actions">
                <button class="btn btn-primary" type="submit"><i class="fa-solid fa-paper-plane"></i> Guardar cita</button>
                <button class="btn" style="background:#eef6ff;color:#0b74de" type="button" id="clearAppointments">
                  <i class="fa-solid fa-trash"></i> Limpiar
                </button>
              </div>
            </form>

            <div class="appointment-list" id="appointmentsList"></div>
          </div>
        </div>
      </div>
    </section>

    <section id="virtual">
      <div class="section-title">
        <h2>Consultas virtuales</h2>
        <p>Espacio pensado para teleorientación, mensajes y videollamadas. Puedes enlazarlo luego a WhatsApp, Meet o Zoom.</p>
      </div>
      <div class="card grid-2">
        <div class="soft">
          <h3 style="margin-top:0">Formulario de consulta virtual</h3>
          <form>
            <label for="vname">Nombre</label>
            <input id="vname" type="text" placeholder="Tu nombre">

            <label for="vmail">Correo electrónico</label>
            <input id="vmail" type="email" placeholder="correo@ejemplo.com">

            <label for="vtopic">Tema</label>
            <select id="vtopic">
              <option>Control prenatal</option>
              <option>Dolor o molestias ginecológicas</option>
              <option>Resultados de estudios</option>
              <option>Orientación general</option>
            </select>

            <label for="vmsg">Mensaje</label>
            <textarea id="vmsg" placeholder="Escribe tu consulta"></textarea>

            <div class="form-actions">
              <button class="btn btn-primary" type="button"><i class="fa-solid fa-video"></i> Enviar solicitud</button>
            </div>
          </form>
        </div>

        <div class="soft">
          <h3 style="margin-top:0">Opciones de atención</h3>
          <p style="color:var(--muted); line-height:1.75">
            Usa esta sección para informar a los pacientes sobre la modalidad de consulta virtual, horarios y requisitos.
          </p>
          <span class="pill"><i class="fa-brands fa-whatsapp"></i> WhatsApp</span>
          <span class="pill"><i class="fa-brands fa-google"></i> Google Meet</span>
          <span class="pill"><i class="fa-solid fa-video"></i> Videollamada</span>
          <div class="notice">
            Sugerencia: agrega aquí un enlace real de videollamada cuando tengas el sistema de telemedicina definido.
          </div>
        </div>
      </div>
    </section>

    <section id="contacto">
      <div class="section-title">
        <h2>Contacto y redes sociales</h2>
        <p>Botones de contacto y acceso rápido para compartir la información de la clínica.</p>
      </div>
      <div class="card grid-2">
        <div class="soft">
          <h3 style="margin-top:0">Datos de contacto</h3>
          <p style="line-height:1.8; color:var(--muted); margin:0">
            <strong style="color:var(--text)">Dra. Luciana Martínez Pacheco</strong><br>
            Teléfono: <strong>62503587</strong><br>
            Dirección: <strong>Calle Beni Nº 377</strong><br>
            Atención: Ginecología y obstetricia
          </p>
          <div class="form-actions" style="margin-top:18px">
            <a class="btn btn-primary" href="tel:62503587"><i class="fa-solid fa-phone"></i> Llamar ahora</a>
            <a class="btn" style="background:#eef6ff;color:#0b74de" href="https://wa.me/59162503587" target="_blank" rel="noopener">
              <i class="fa-brands fa-whatsapp"></i> WhatsApp
            </a>
          </div>
        </div>

        <div class="soft">
          <h3 style="margin-top:0">Redes sociales</h3>
          <div class="social">
            <a href="https://facebook.com" target="_blank" rel="noopener" aria-label="Facebook"><i class="fa-brands fa-facebook-f"></i></a>
            <a href="https://instagram.com" target="_blank" rel="noopener" aria-label="Instagram"><i class="fa-brands fa-instagram"></i></a>
            <a href="https://youtube.com" target="_blank" rel="noopener" aria-label="YouTube"><i class="fa-brands fa-youtube"></i></a>
            <a href="https://tiktok.com" target="_blank" rel="noopener" aria-label="TikTok"><i class="fa-brands fa-tiktok"></i></a>
          </div>
          <div class="notice">
            Estos iconos están listos para enlazar las cuentas reales de la clínica.
          </div>
        </div>
      </div>
    </section>
  </main>

  <div class="floating">
    <a class="wa" href="https://wa.me/59162503587" target="_blank" rel="noopener" title="WhatsApp"><i class="fa-brands fa-whatsapp"></i></a>
    <a class="mapbtn" href="#ubicacion" title="Ir a ubicación"><i class="fa-solid fa-location-dot"></i></a>
  </div>

  <footer class="footer">
    <div class="wrap">
      © 2026 Clínica Ginecológica y Obstétrica — Dra. Luciana Martínez Pacheco
    </div>
  </footer>

  <script>
    const dowEl = document.getElementById("dow");
    const gridEl = document.getElementById("calendarGrid");
    const monthLabel = document.getElementById("monthLabel");
    const todayLabel = document.getElementById("todayLabel");
    const dateInput = document.getElementById("date");
    const appointmentsList = document.getElementById("appointmentsList");
    const form = document.getElementById("appointmentForm");

    const prevBtn = document.getElementById("prevMonth");
    const nextBtn = document.getElementById("nextMonth");
    const clearBtn = document.getElementById("clearAppointments");

    const dows = ["Dom", "Lun", "Mar", "Mié", "Jue", "Vie", "Sáb"];
    const months = ["Enero","Febrero","Marzo","Abril","Mayo","Junio","Julio","Agosto","Septiembre","Octubre","Noviembre","Diciembre"];

    let view = new Date();
    view.setDate(1);
    let selectedDate = null;

    function storageKey(){
      return "clinica_citas_avanzado";
    }

    function fmtDate(date){
      return date.toLocaleDateString("es-BO", {weekday:"long", year:"numeric", month:"long", day:"numeric"});
    }

    function isoDate(date){
      const y = date.getFullYear();
      const m = String(date.getMonth()+1).padStart(2,"0");
      const d = String(date.getDate()).padStart(2,"0");
      return `${y}-${m}-${d}`;
    }

    function loadAppointments(){
      try { return JSON.parse(localStorage.getItem(storageKey()) || "[]"); }
      catch { return []; }
    }

    function saveAppointments(items){
      localStorage.setItem(storageKey(), JSON.stringify(items));
    }

    function renderAppointments(){
      const items = loadAppointments();
      if(!items.length){
        appointmentsList.innerHTML = `<div class="appointment"><strong>No hay citas guardadas</strong><span>Las citas que registres aparecerán aquí.</span></div>`;
        return;
      }
      appointmentsList.innerHTML = items.map((a, idx) => `
        <div class="appointment">
          <strong>${a.name} — ${a.date} ${a.time ? "• " + a.time : ""}</strong>
          <span>Teléfono: ${a.phone}<br>Motivo: ${a.reason || "Sin detalle"}<br>Registro #${idx + 1}</span>
        </div>
      `).join("");
    }

    function renderDOW(){
      dowEl.innerHTML = dows.map(d => `<div class="dow">${d}</div>`).join("");
    }

    function renderCalendar(){
      const year = view.getFullYear();
      const month = view.getMonth();
      const firstDay = new Date(year, month, 1);
      const start = new Date(firstDay);
      start.setDate(1 - firstDay.getDay());

      const today = new Date();
      monthLabel.textContent = `${months[month]} ${year}`;
      todayLabel.textContent = `Hoy: ${fmtDate(today)}`;

      const cells = [];
      for(let i=0; i<42; i++){
        const d = new Date(start);
        d.setDate(start.getDate() + i);
        const isCurrentMonth = d.getMonth() === month;
        const isToday = isoDate(d) === isoDate(today);
        const isSelected = selectedDate && isoDate(d) === selectedDate;

        cells.push(`
          <button type="button"
            class="day ${isCurrentMonth ? "" : "muted"} ${isSelected ? "selected" : ""}"
            data-date="${isoDate(d)}"
            ${isCurrentMonth ? "" : "disabled"}
            aria-label="${fmtDate(d)}">
            <strong>${d.getDate()}</strong>
            <small>${isToday ? '<span class="dot"></span> Hoy' : (isCurrentMonth ? 'Disponible' : '')}</small>
          </button>
        `);
      }
      gridEl.innerHTML = cells.join("");

      gridEl.querySelectorAll(".day:not(.muted)").forEach(btn => {
        btn.addEventListener("click", () => {
          selectedDate = btn.dataset.date;
          dateInput.value = selectedDate;
          renderCalendar();
        });
      });
    }

    prevBtn.addEventListener("click", () => {
      view.setMonth(view.getMonth() - 1);
      renderCalendar();
    });

    nextBtn.addEventListener("click", () => {
      view.setMonth(view.getMonth() + 1);
      renderCalendar();
    });

    clearBtn.addEventListener("click", () => {
      if(confirm("¿Eliminar todas las citas guardadas en este navegador?")){
        localStorage.removeItem(storageKey());
        renderAppointments();
        form.reset();
        dateInput.value = "";
        selectedDate = null;
        renderCalendar();
      }
    });

    form.addEventListener("submit", (e) => {
      e.preventDefault();
      const name = document.getElementById("name").value.trim();
      const phone = document.getElementById("phone").value.trim();
      const date = document.getElementById("date").value.trim();
      const time = document.getElementById("time").value.trim();
      const reason = document.getElementById("reason").value.trim();

      if(!name || !phone || !date || !time){
        alert("Completa nombre, teléfono, fecha y hora.");
        return;
      }

      const items = loadAppointments();
      items.unshift({ name, phone, date, time, reason });
      saveAppointments(items.slice(0, 10)); // guarda hasta 10 citas visibles
      renderAppointments();
      alert("Cita guardada en el calendario del navegador.");
      form.reset();
      dateInput.value = "";
      selectedDate = null;
      renderCalendar();
    });

    renderDOW();
    renderCalendar();
    renderAppointments();
  </script>
</body>
</html>
