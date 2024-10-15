<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Yerba Mate Mística</title>
  <style>
    /* Estilos generales */
    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      background-color: #ffe6f0; /* Fondo rosa claro */
      color: #333;
    }

    /* Encabezado */
    header {
      background-color: #ff99c1; /* Fondo rosa claro */
      color: #fff;
      padding: 1.5rem;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    header h1 {
      font-size: 2.8rem;
      margin: 0;
      font-weight: 700;
    }

    header nav ul {
      list-style: none;
      display: flex;
      justify-content: center;
      padding: 0;
    }

    header nav ul li {
      margin: 0 20px;
    }

    header nav ul li a {
      color: white;
      text-decoration: none;
      font-size: 1.2rem;
      font-weight: bold;
      transition: color 0.3s;
    }

    header nav ul li a:hover {
      color: #ffe6f0; /* Cambio de color al pasar el ratón */
    }

    /* Sección de Introducción */
    .intro {
      text-align: center;
      padding: 4rem;
      background: linear-gradient(135deg, #ffb3d9, #ff99c1); /* Degradado rosa claro */
      color: #fff;
      border-bottom: 5px solid #ff99c1; /* Borde inferior */
    }

    .intro h2 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
      animation: textFadeIn 3s ease-in-out;
    }

    .intro p {
      font-size: 1.2rem;
      margin-bottom: 2rem;
      animation: textFadeIn 4s ease-in-out;
    }

    .intro img {
      width: 100%;
      max-width: 550px;
      display: block;
      margin: 1rem auto;
      border-radius: 10px;
      animation: zoomIn 2s ease-in-out;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Sombra de imagen */
    }

    /* Animaciones */
    @keyframes zoomIn {
      from {
        transform: scale(0.5);
        opacity: 0;
      }
      to {
        transform: scale(1);
        opacity: 1;
      }
    }

    @keyframes textFadeIn {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
    }

    /* Sección de Proceso */
    .process {
      padding: 3rem;
      background-color: #fff; /* Fondo blanco */
      border-bottom: 5px solid #ff99c1; /* Borde inferior */
    }

    .process h2 {
      text-align: center;
      font-size: 2.5rem;
      margin-bottom: 2rem;
      animation: slideInFromLeft 1s ease-in-out;
    }

    .process-step {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1.5rem;
      background-color: #ffb3d9; /* Fondo rosa claro */
      margin: 1.5rem auto;
      border-radius: 10px;
      max-width: 900px;
      transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
    }

    .process-step img {
      width: 150px;
      margin-right: 1rem;
      border-radius: 10px; /* Bordes redondeados en imágenes */
    }

    .process-step:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    }

    @keyframes slideInFromLeft {
      from {
        transform: translateX(-100%);
        opacity: 0;
      }
      to {
        transform: translateX(0);
        opacity: 1;
      }
    }

    /* Sección de Valores */
    .value-section {
      padding: 3rem;
      background-color: #ff99c1; /* Fondo rosa claro */
      color: #333;
    }

    .value-section h2 {
      text-align: center;
      font-size: 2.5rem;
      margin-bottom: 2rem;
    }

    .value-box {
      background-color: #fff; /* Fondo blanco */
      padding: 2rem;
      margin: 1.5rem auto;
      max-width: 800px;
      border-left: 5px solid #ff99c1;
      transition: background-color 0.3s ease-in-out, transform 0.3s ease-in-out;
      animation: slideInFromRight 1.5s ease-in-out;
      border-radius: 10px; /* Bordes redondeados en las cajas */
    }

    .value-box:hover {
      background-color: #ffe6f0; /* Cambio a rosa claro al pasar el ratón */
      transform: translateY(-5px); /* Efecto de elevar la caja al pasar el ratón */
    }

    @keyframes slideInFromRight {
      from {
        transform: translateX(100%);
        opacity: 0;
      }
      to {
        transform: translateX(0);
        opacity: 1;
      }
    }

    /* Sección de Contacto */
    .contact-section {
      padding: 4rem;
      background-color: #ff99c1; /* Fondo rosa claro */
      color: white;
      text-align: center;
    }

    .contact-section h2 {
      margin-bottom: 1.5rem;
      font-size: 2.5rem;
    }

    form {
      display: flex;
      flex-direction: column;
      align-items: center;
      max-width: 400px;
      margin: 0 auto;
    }

    form input, form textarea {
      width: 100%;
      padding: 0.8rem;
      margin: 0.5rem 0;
      border-radius: 5px;
      border: none;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    form button {
      background-color: white;
      color: #ff99c1; /* Color rosa claro */
      padding: 0.8rem 1.5rem;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-size: 1.2rem;
      transition: background-color 0.3s, transform 0.3s;
    }

    form button:hover {
      background-color: #ffe6f0; /* Fondo rosa claro al pasar el ratón */
      transform: scale(1.05); /* Efecto de aumento en el botón al pasar el ratón */
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 1rem;
      background-color: #333;
      color: #fff;
      position: relative; /* Posicionamiento relativo */
      bottom: 0; /* Posicionamiento en la parte inferior */
      width: 100%; /* Ancho completo */
    }

    /* Media Queries para pantallas pequeñas */
    @media (max-width: 768px) {
      header nav ul {
        flex-direction: column;
        padding: 1rem 0;
      }

      header nav ul li {
        margin: 10px 0;
      }

      .intro h2 {
        font-size: 2rem;
      }

      .intro p {
        font-size: 1rem;
      }

      .process h2,
      .value-section h2 {
        font-size: 2rem;
      }

      .value-box,
      .process-step {
        flex-direction: column; /* Cambiar a columna en pantallas pequeñas */
        align-items: center;
      }

      .process-step img {
        width: 120px; /* Ajustar tamaño de imagen */
      }

      .contact-section h2 {
        font-size: 2rem;
      }

      form button {
        font-size: 1rem;
      }
    }

    @media (max-width: 480px) {
      header h1 {
        font-size: 2.2rem;
      }

      header nav ul li a {
        font-size: 1rem;
      }

      .intro h2 {
        font-size: 1.8rem;
      }

      .intro p {
        font-size: 0.9rem;
      }

      .process h2,
      .value-section h2 {
        font-size: 1.8rem;
      }

      .value-box,
      .process-step {
        max-width: 100%; /* Ancho completo en pantallas muy pequeñas */
      }
    }
  </style>
</head>
<body>

  <!-- Encabezado -->
  <header>
    <h1>Yerba Mate Mística</h1>
    <nav>
      <ul>
        <li><a href="#introduccion">Introducción</a></li>
        <li><a href="#proceso">Proceso</a></li>
        <li><a href="#valores">Valores</a></li>
        <li><a href="#contacto">Contacto</a></li>
      </ul>
    </nav>
  </header>

  <!-- Sección 1: Introducción -->
  <section id="introduccion" class="intro">
    <h2>Bienvenidos a Yerba Mate Mística</h2>
    <p>Descubre la esencia de nuestra yerba mate, cultivada con amor y tradición.</p>
    <img src="fotos/4.jpeg" alt="Yerba Mate">
  </section>

  <!-- Sección 2: Proceso -->
  <section id="proceso" class="process">
    <h2>Nuestro Proceso</h2>
    <div class="process-step">
      <img src="fotos/1.jpeg" alt="Materia Prima">
      <div>
        <h3>Materia Prima</h3>
        <p>Seleccionamos las mejores hojas de yerba mate de los cultivos locales.</p>
      </div>
    </div>
    <div class="process-step">
      <img src="fotos/3.jpeg" alt="Secado de Hojas">
      <div>
        <h3>Secado de Hojas</h3>
        <p>Las hojas se secan al aire para resaltar su sabor natural y aroma.</p>
      </div>
    </div>
    <div class="process-step">
      <img src="fotos/3.jpeg" alt="Molienda">
      <div>
        <h3>Molienda</h3>
        <p>Las hojas secas se muelen para obtener la textura perfecta para el consumo.</p>
      </div>
    </div>
  </section>

  <!-- Sección 3: Valores -->
  <section id="valores" class="value-section">
    <h2>Nuestros Valores</h2>
    <div class="value-box">
      <h3>Calidad</h3>
      <p>Nos comprometemos a ofrecer la mejor calidad en cada taza de yerba mate.</p>
    </div>
    <div class="value-box">
      <h3>Sustentabilidad</h3>
      <p>Practicamos métodos de producción sostenibles que cuidan el medio ambiente.</p>
    </div>
    <div class="value-box">
      <h3>Tradición</h3>
      <p>Respetamos las tradiciones de la yerba mate, fusionando lo antiguo con lo moderno.</p>
    </div>
  </section>

  <!-- Sección 4: Contacto -->
  <section id="contacto" class="contact-section">
    <h2>Contáctanos</h2>
    <form>
      <input type="text" placeholder="Tu nombre" required>
      <input type="email" placeholder="Tu correo electrónico" required>
      <textarea placeholder="Tu mensaje" rows="4" required></textarea>
      <button type="submit">Enviar</button>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2024 Yerba Mate Mística. Todos los derechos reservados.</p>
  </footer>

</body>
</html>
