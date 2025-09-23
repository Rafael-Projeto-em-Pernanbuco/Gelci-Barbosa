<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Gelci Barbosa do Pife - Exu-PE</title>
  <style>
    body {
      background-color: #FFD700; /* Amarelo */
      color: white;
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #4682B4; /* Azul claro */
      padding: 20px;
      text-align: center;
    }

    header h1 {
      margin: 0;
      color: white;
    }

    section {
      padding: 20px;
    }

    .button {
      background-color: #87CEFA; /* Azul claro */
      color: white;
      padding: 10px 20px;
      border: none;
      cursor: pointer;
      margin-top: 10px;
    }

    .social-icons a {
      margin: 0 10px;
      color: white;
      text-decoration: none;
      font-size: 24px;
    }

    .map-container {
      margin-top: 20px;
    }

    footer {
      background-color: #333;
      color: white;
      padding: 10px;
      text-align: center;
    }

    input[type="email"] {
      padding: 10px;
      width: 250px;
    }

    .audio-recorder {
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Gelci Barbosa do Pife - Exu, PE</h1>
  </header>

  <!-- Google Tradutor -->
  <div id="google_translate_element" style="text-align: right; padding: 10px;"></div>
  <script type="text/javascript">
    function googleTranslateElementInit() {
      new google.translate.TranslateElement({pageLanguage: 'pt'}, 'google_translate_element');
    }
  </script>
  <script src="https://translate.google.com/translate_a/element.js?cb=googleTranslateElementInit"></script>

  <section>
    <h2>Localização</h2>
    <div class="map-container">
      <iframe
        src="https://www.google.com/maps?q=Exu,PE&output=embed"
        width="100%"
        height="300"
        style="border:0;"
        allowfullscreen=""
        loading="lazy">
      </iframe>
    </div>

    <h2>Cadastro de E-mail</h2>
    <form>
      <input type="email" placeholder="Seu e-mail" required />
      <button class="button" type="submit">Cadastrar</button>
    </form>

    <h2>Gravador de Áudio</h2>
    <div class="audio-recorder">
      <button class="button" onclick="startRecording()">Gravar</button>
      <button class="button" onclick="stopRecording()">Parar</button>
      <audio id="audioPlayback" controls></audio>
    </div>

    <h2>Redes Sociais</h2>
    <div class="social-icons">
      <a href="https://facebook.com" target="_blank">Facebook</a>
      <a href="https://instagram.com" target="_blank">Instagram</a>
      <a href="https://www.kwai.com/" target="_blank">Kwai</a>
      <a href="https://tiktok.com" target="_blank">TikTok</a>
      <a href="https://twitter.com" target="_blank">Twitter</a>
      <a href="https://t.me" target="_blank">Telegram</a>
      <a href="https://youtube.com" target="_blank">YouTube</a>
      <a href="https://wa.me/5587999999999" target="_blank">WhatsApp</a>
    </div>
  </section>

  <!-- Chat online via Tawk.to -->
  <script type="text/javascript">
    var Tawk_API=Tawk_API||{}, Tawk_LoadStart=new Date();
    (function(){
      var s1=document.createElement("script"),s0=document.getElementsByTagName("script")[0];
      s1.async=true;
      s1.src='https://embed.tawk.to/your_tawkto_id/1abc123'; // Substitua com seu ID do Tawk.to
      s1.charset='UTF-8';
      s1.setAttribute('crossorigin','*');
      s0.parentNode.insertBefore(s1,s0);
    })();
  </script>

  <!-- Gravador de áudio com JavaScript -->
  <script>
    let mediaRecorder;
    let audioChunks = [];

    async function startRecording() {
      const stream = await navigator.mediaDevices.getUserMedia({ audio: true });
      mediaRecorder = new MediaRecorder(stream);
      mediaRecorder.start();

      mediaRecorder.ondataavailable = (event) => {
        audioChunks.push(event.data);
      };

      mediaRecorder.onstop = () => {
        const audioBlob = new Blob(audioChunks, { type: 'audio/mpeg' });
        const audioUrl = URL.createObjectURL(audioBlob);
        const audio = document.getElementById('audioPlayback');
        audio.src = audioUrl;
        audioChunks = [];
      };
    }

    function stopRecording() {
      if (mediaRecorder) {
        mediaRecorder.stop();
      }
    }
  </script>

  <footer>
    &copy; 2025 Gelci Barbosa do Pife - Todos os direitos reservados
  </footer>
</body>
</html>
