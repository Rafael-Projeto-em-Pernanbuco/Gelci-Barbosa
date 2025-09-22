<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Gelci Barbosa do Pife - Exu-PE</title>

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">

  <!-- Ícones das Redes Sociais - Font Awesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" integrity="sha512-xh6xzW5hdbmhZhcuqVlgZZUnF64y/1JXtXUvDoVgr+c3Zwqv+uNQeYv0TkO/jU3+hJWWTnU9YzPnBbYY+1rQKQ==" crossorigin="anonymous" referrerpolicy="no-referrer" />

  <!-- Estilos -->
  <style>
    body {
      margin: 0;
      font-family: 'Roboto', sans-serif;
      background-color: #FFD700; /* Amarelo escuro */
      color: white;
    }

    header {
      background-color: #002147; /* Azul escuro */
      text-align: center;
      padding: 20px;
    }

    header h1 {
      margin: 0;
      font-size: 2em;
    }

    .tradutor {
      position: absolute;
      top: 10px;
      right: 10px;
    }

    .container {
      padding: 20px;
      background-color: #FFD700;
    }

    iframe {
      width: 100%;
      height: 400px;
      border: none;
      margin-top: 20px;
    }

    footer {
      background-color: #002147;
      text-align: center;
      padding: 20px;
    }

    .redes-sociais {
      margin-top: 20px;
      text-align: center;
    }

    .redes-sociais a {
      margin: 10px;
      font-size: 28px;
      color: white;
      text-decoration: none;
      transition: transform 0.2s;
    }

    .redes-sociais a:hover {
      transform: scale(1.2);
    }

    h2 {
      color: #002147;
      background-color: white;
      padding: 10px;
      border-radius: 5px;
      display: inline-block;
    }

    p {
      font-size: 1.2em;
    }
  </style>
</head>
<body>

  <!-- Google Tradutor -->
  <div class="tradutor" id="google_translate_element"></div>

  <header>
    <h1>Gelci Barbosa do Pife</h1>
    <p>Exu - Pernambuco</p>
  </header>

  <div class="container">
    <h2>Sobre</h2>
    <p>Bem-vindo ao site oficial de Gelci Barbosa do Pife, músico tradicional da cidade de Exu-PE.</p>

    <h2>Localização</h2>
    <!-- Mapa do Google Maps focado em Exu-PE -->
    <iframe 
      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1978.4212467682397!2d-39.72427595473083!3d-7.513025721946219!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x7a2cd10509f3637%3A0xcfe1eb70f8147f13!2sExu%2C%20PE%2C%2056320-000!5e0!3m2!1spt-BR!2sbr!4v1695392671230!5m2!1spt-BR!2sbr" 
      allowfullscreen=""
      loading="lazy"
      referrerpolicy="no-referrer-when-downgrade">
    </iframe>

    <div class="redes-sociais">
      <h2>Redes Sociais</h2>
      <br><br>
      <a href="https://instagram.com/" target="_blank" title="Instagram">
        <i class="fab fa-instagram"></i>
      </a>
      <a href="https://facebook.com/" target="_blank" title="Facebook">
        <i class="fab fa-facebook"></i>
      </a>
      <a href="https://wa.me/seunumerodetelefone" target="_blank" title="WhatsApp">
        <i class="fab fa-whatsapp"></i>
      </a>
      <a href="https://tiktok.com/" target="_blank" title="TikTok">
        <i class="fab fa-tiktok"></i>
      </a>
      <a href="https://www.kwai.com/" target="_blank" title="Kwai">
        <i class="fas fa-video"></i> <!-- Kwai não tem ícone oficial no Font Awesome -->
      </a>
      <a href="https://t.me/seuusuario" target="_blank" title="Telegram">
        <i class="fab fa-telegram"></i>
      </a>
      <a href="https://twitter.com/" target="_blank" title="Twitter/X">
        <i class="fab fa-x-twitter"></i>
      </a>
    </div>
  </div>

  <footer>
    <p>&copy; 2025 Gelci Barbosa do Pife. Todos os direitos reservados.</p>
  </footer>

  <!-- Script do Google Tradutor -->
  <script type="text/javascript">
    function googleTranslateElementInit() {
      new google.translate.TranslateElement({
        pageLanguage: 'pt',
        includedLanguages: 'en,es,fr,it,de,pt',
        layout: google.translate.TranslateElement.InlineLayout.SIMPLE
      }, 'google_translate_element');
    }
  </script>
  <script type="text/javascript" 
    src="//translate.google.com/translate_a/element.js?cb=googleTranslateElementInit">
  </script>

</body>
</html>
