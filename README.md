<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>eBook Iluminação Estratégica - Download Gratuito</title>
  <style>
    body {
      background-color: #0d0d0d;
      color: #ffffff;
      font-family: 'Helvetica Neue', sans-serif;
      padding: 40px 20px;
      text-align: center;
    }
    h1 {
      color: #f1c40f;
      font-size: 2.5em;
      margin-bottom: 10px;
    }
    p {
      font-size: 1.2em;
      max-width: 600px;
      margin: 0 auto 30px auto;
    }
    form {
      max-width: 500px;
      margin: 0 auto;
    }
    input, select, button {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      border: none;
      border-radius: 8px;
      font-size: 1em;
    }
    input, select {
      background-color: #1c1c1c;
      color: #fff;
    }
    button {
      background-color: #f1c40f;
      color: #000;
      cursor: pointer;
      font-weight: bold;
      transition: background-color 0.3s ease;
    }
    button:hover {
      background-color: #e0b207;
    }
    .footer {
      margin-top: 40px;
      font-size: 0.9em;
      color: #888;
    }

    @media (max-width: 768px) {
      h1 {
        font-size: 2em;
      }
    }
  </style>
</head>
<body>

  <h1>Receba o eBook “Iluminação Estratégica”</h1>
  <p>Transforme seu espaço comercial com técnicas de iluminação que aumentam vendas, valorizam produtos e criam experiências memoráveis.</p>

  <form action="https://formspree.io/f/xdkgypea" method="POST" onsubmit="enviar(event)">
    <input type="text" name="nome" placeholder="Seu nome" required />
    <input type="email" name="email" placeholder="Seu e-mail" required />
    
    <select name="segmento" required>
      <option value="">Qual é o segmento do seu negócio?</option>
      <option value="moda">Moda (loja de roupas, calçados, acessórios)</option>
      <option value="beleza">Beleza e estética</option>
      <option value="saude">Saúde (clínicas, consultórios, farmácias)</option>
      <option value="alimentacao">Alimentação (cafeterias, restaurantes, bares)</option>
      <option value="servicos">Serviços em geral</option>
      <option value="varejo">Varejo em geral</option>
      <option value="joias">Joias e semi-joias</option>
      <option value="moveis">Móveis e decoração</option>
      <option value="automotivo">Automotivo (showrooms, oficinas)</option>
      <option value="esportes">Esporte, saúde e bem-estar</option>
      <option value="outro">Outro</option>
    </select>

    <button type="submit">Quero receber o eBook</button>
  </form>

  <div class="footer">
    © 2025 Arquiteto Lucio Meireles — Todos os direitos reservados.
  </div>

  <script>
    function enviar(e) {
      e.preventDefault();
      const form = e.target;
      const data = new FormData(form);

      fetch(form.action, {
        method: 'POST',
        body: data,
        headers: {
          'Accept': 'application/json'
        }
      }).then(response => {
        if (response.ok) {
          alert('Enviado com sucesso! Você será redirecionado para o download do eBook.');
          window.location.href = 'https://drive.google.com/file/d/1Jp_HoyRZSsiqpKTw3eQazdcdyxyvSmvv/view?usp=drive_link';
        } else {
          alert('Erro ao enviar. Verifique os dados ou tente novamente mais tarde.');
        }
      });
    }
  </script>

</body>
</html>
