<!-- Indica al navegador que estamos utilizando el estándar HTML5 -->
<!DOCTYPE html>

<!-- Define el idioma principal del documento como español -->
<html lang="es">

<head>
  <!-- Permite caracteres especiales en español como tildes o la letra ñ -->
  <meta charset="UTF-8">

  <!-- Hace que la web sea adaptable (responsive) a teléfonos móviles y tablets -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- Título que se muestra en la pestaña del navegador -->
  <title>Portfolio | Tu Nombre - Estudiante de DAM</title>

  <!-- Enlace a tu archivo local de estilos CSS -->
  <link rel="stylesheet" href="style.css">

  <!-- Carga la librería FontAwesome desde CDN (nube). 
       Gracias a esto NO necesitas descargar iconos de Java, GitHub, Android, etc. -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>

<body>

  <!-- ===================================================
       BARRA DE NAVEGACIÓN SUPERIOR (NAVBAR)
       Permite saltar a las secciones con enlaces de ancla (#)
  ==================================================== -->
  <nav class="navbar">
    <!-- Logotipo o texto identificativo -->
    <div class="logo">&lt;TuNombre /&gt;</div>

    <!-- Lista de enlaces de navegación -->
    <ul class="nav-links">
      <!-- Los enlaces href="#id" hacen scroll automático a la sección con ese id -->
      <li><a href="#proyectos">Proyectos</a></li>
      <li><a href="#estudios">Estudios</a></li>
      <li><a href="#experiencia">Experiencia</a></li>
      <li><a href="#contacto">Contacto</a></li>
    </ul>
  </nav>

  <!-- ===================================================
       SECCIÓN PRINCIPAL (HERO)
       Muestra foto, nombre, descripción, redes y descarga de CV
  ==================================================== -->
  <header class="hero">
    <div class="hero-content">

      <!-- IMAGEN DE PERFIL O AVATAR:
           Opción 1 (Tu propia imagen descargada): pon src="assets/avatar.png"
           Opción 2 (Imagen temporal de internet): dejamos este enlace de ejemplo -->
      <img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=300&q=80" 
           alt="Foto o avatar del estudiante" 
           class="avatar">

      <!-- Nombre y apellidos del estudiante -->
      <h1>Hola, soy <span>Tu Nombre y Apellidos</span></h1>

      <!-- Subtítulo profesional enfocado a DAM -->
      <p class="subtitle">Estudiante de 2º de DAM | Desarrollador Multiplataforma</p>
      
      <!-- ENLACES A REDES SOCIALES Y CORREO:
           En 'href' pones la dirección completa de tus perfiles.
           target="_blank" abre la página en una pestaña nueva.
           rel="noopener noreferrer" es por seguridad al abrir enlaces externos. -->
      <div class="social-links">
        <!-- Enlace a tu perfil de GitHub -->
        <a href="https://github.com/tu-usuario" target="_blank" rel="noopener noreferrer" title="GitHub">
          <i class="fab fa-github"></i>
        </a>

        <!-- Enlace a tu perfil de LinkedIn -->
        <a href="https://linkedin.com/in/tu-usuario" target="_blank" rel="noopener noreferrer" title="LinkedIn">
          <i class="fab fa-linkedin"></i>
        </a>

        <!-- Enlace a tu correo: al hacer clic abre la app de correo del usuario -->
        <a href="mailto:tu-correo@gmail.com" title="Enviar correo electrónico">
          <i class="fas fa-envelope"></i>
        </a>
      </div>

      <!-- BOTÓN PARA DESCARGAR EL CV:
           - El atributo 'download' indica al navegador que debe descargar el archivo en vez de abrirlo.
           - En 'href' pones la ruta donde tengas tu PDF (ejemplo: assets/tu_curriculum.pdf).
           - Si lo subes a Google Drive, cambia 'download' y pon el enlace público de Drive. -->
      <a href="assets/tu_curriculum.pdf" download="CV_TuNombre.pdf" class="btn-cv">
        <i class="fas fa-download"></i> Descargar CV
      </a>

    </div>
  </header>

  <!-- ===================================================
       CONTENIDO PRINCIPAL
  ==================================================== -->
  <main>

    <!-- SECCIÓN DE HABILIDADES TÉCNICAS (STACK)
         Los iconos no requieren descargas; se definen con clases FontAwesome -->
    <section class="section">
      <h2>Tecnologías</h2>
      <div class="skills-icons">
        <div class="skill-item">
          <i class="fab fa-java"></i>
          <span>Java</span>
        </div>
        <div class="skill-item">
          <i class="fab fa-android"></i>
          <span>Android</span>
        </div>
        <div class="skill-item">
          <i class="fas fa-database"></i>
          <span>SQL</span>
        </div>
        <div class="skill-item">
          <i class="fab fa-git-alt"></i>
          <span>Git</span>
        </div>
      </div>
    </section>

    <!-- SECCIÓN DE PROYECTOS REALIZADOS
         id="proyectos" coincide con el enlace del menú superior -->
    <section id="proyectos" class="section">
      <h2>Proyectos</h2>
      
      <div class="grid-cards">

        <!-- TARJETA DEL PROYECTO 1 -->
        <article class="card">
          <!-- IMAGEN DE PREVISUALIZACIÓN:
               Opción A: captura propia guardada en 'assets/proyecto1.png'.
               Opción B: enlace de imagen de internet mientras pruebas (usado aquí). -->
          <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?auto=format&fit=crop&w=600&q=80" 
               alt="Captura de pantalla de la App Móvil" 
               class="card-img">

          <div class="card-body">
            <h3>App de Gestión de Tareas (Android)</h3>
            <p>Aplicación móvil desarrollada en Kotlin y Java con persistencia local mediante Room / SQLite y diseño Material 3.</p>
            
            <!-- Etiquetas de las tecnologías utilizadas -->
            <div class="tags">
              <span>Kotlin</span>
              <span>Android</span>
              <span>SQLite</span>
            </div>

            <!-- Enlace que lleva al repositorio del proyecto -->
            <a href="https://github.com/tu-usuario/proyecto-android" target="_blank" rel="noopener noreferrer" class="card-link">
              <i class="fab fa-github"></i> Ver Código en GitHub
            </a>
          </div>
        </article>

        <!-- TARJETA DEL PROYECTO 2 -->
        <article class="card">
          <!-- Imagen de prueba para el segundo proyecto -->
          <img src="https://images.unsplash.com/photo-1507238691740-187a5b1d37b8?auto=format&fit=crop&w=600&q=80" 
               alt="Captura de pantalla del Proyecto de Escritorio" 
               class="card-img">

          <div class="card-body">
            <h3>Sistema de Gestión de Clientes</h3>
            <p>Aplicación de escritorio multiplataforma desarrollada en Java con interfaz JavaFX y conexión a base de datos MySQL.</p>
            
            <div class="tags">
              <span>Java</span>
              <span>JavaFX</span>
              <span>MySQL</span>
            </div>

            <a href="https://github.com/tu-usuario/proyecto-escritorio" target="_blank" rel="noopener noreferrer" class="card-link">
              <i class="fab fa-github"></i> Ver Código en GitHub
            </a>
          </div>
        </article>

      </div>
    </section>

    <!-- SECCIÓN DE ESTUDIOS
         id="estudios" coincide con el menú superior -->
    <section id="estudios" class="section">
      <h2>Estudios</h2>
      
      <div class="timeline">
        <!-- Estudio actual (DAM) -->
        <div class="timeline-item">
          <h3>C.F.G.S. Desarrollo de Aplicaciones Multiplataforma</h3>
          <p class="institute">IES / Centro Educativo | <em>2024 - Actualidad</em></p>
          <p>Formación actual enfocada en desarrollo en entornos móviles, acceso a datos, sistemas ERP y diseño de interfaces.</p>
        </div>

        <!-- Estudio previo (Bachillerato, Grado Medio, etc.) -->
        <div class="timeline-item">
          <h3>Bachillerato Tecnológico / Ciclo Formativo de Grado Medio</h3>
          <p class="institute">IES / Centro de procedencia | <em>2022 - 2024</em></p>
          <p>Formación académica previa orientada a bases técnicas y científicas.</p>
        </div>
      </div>
    </section>

    <!-- SECCIÓN DE EXPERIENCIA LABORAL
         id="experiencia" coincide con el menú superior -->
    <section id="experiencia" class="section">
      <h2>Experiencia</h2>
      
      <div class="timeline">
        <!-- Si no tienes contratos previos, enfócalo hacia las prácticas FCT -->
        <div class="timeline-item">
          <h3>Búsqueda de Prácticas FCT (Desarrollador Junior)</h3>
          <p class="institute">Periodo previsto: 2026 | Modalidad: Presencial / Remoto</p>
          <p>Preparado para realizar la Formación en Centros de Trabajo (FCT) en puestos de desarrollo multiplataforma, soporte o desarrollo backend/móvil.</p>
        </div>
      </div>
    </section>

  </main>

  <!-- ===================================================
       PIE DE PÁGINA (FOOTER)
  ==================================================== -->
  <footer id="contacto">
    <p>Diseñado por Tu Nombre y Apellidos © 2026</p>
  </footer>

</body>
</html>