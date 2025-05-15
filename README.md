<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Iluminação Estratégica - eBook Gratuito</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --cinza-escuro: #3A4550;
      --cinza-medio: #7E8C97;
      --cinza-claro: #B1B9C1;
      --branco: #f9f9f9;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Montserrat', sans-serif;
      background-color: var(--cinza-escuro);
      color: var(--cinza-escuro);
    }

    .wrapper {
      max-width: 1200px;
      margin: 0 auto;
      padding: 60px 40px;
      background-color: var(--branco);
      box-shadow: 0 0 60px rgba(0,0,0,0.1);
      border-radius: 16px;
    }

    .logo {
      text-align: center;
      font-size: 1rem;
      font-weight: 600;
      letter-spacing: 2px;
      color: var(--cinza-medio);
      margin-bottom: 40px;
    }

    .hero {
      text-align: center;
      margin-bottom: 40px;
    }

    .hero h1 {
      font-size: 2.8rem;
      font-weight: 700;
      color: var(--cinza-escuro);
      margin-bottom: 20px;
    }

    .hero span {
      color: var(--cinza-medio);
    }

    .hero p {
      font-size: 1.2rem;
      color: var(--cinza-medio);
      max-width: 600px;
      margin: 0 auto 30px;
    }

    .btn {
      background-color: var(--cinza-medio);
      color: white;
      padding: 16px 36px;
      font-size: 1rem;
      font-weight: 600;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .btn:hover {
      background-color: #6a7886;
    }

    .benefits {
      display: flex;
      justify-content: space-around;
      margin: 60px 0;
      gap: 20px;
      flex-wrap: wrap;
    }

    .benefit {
      background-color: var(--cinza-escuro);
      color: white;
      border-radius: 12px;
      padding: 24px;
      flex: 1;
      min-width: 250px;
      opacity: 0.9;
      transition: opacity 0.4s ease, transform 0.4s ease;
    }

    .benefit:hover {
      opacity: 1;
      transform: translateY(-5px);
    }

    .form-section {
      max-width: 600px;
      margin: 0 auto 60px;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 20px;
    }

    input, select {
      padding: 14px 20px;
      font-size: 1rem;
      border-radius: 10px;
      border: 1px solid var(--cinza-claro);
    }

    .testimonial {
      background-color: var(--cinza-claro);
      padding: 24px;
      border-left: 5px solid var(--cinza-medio);
      font-style: italic;
      margin: 40px auto;
      max-width: 600px;
      color: var(--cinza-escuro);
      opacity: 0.9;
      transition: opacity 0.4s ease, transform 0.4s ease;
    }

    .testimonial:hover {
      opacity: 1;
      transform: scale(1.02);
    }

    .about {
      background-color: var(--cinza-medio);
      color: white;
      padding: 40px;
      border-radius: 12px;
      margin: 60px auto;
      max-width: 800px;
      text-align: center;
    }

    .about h2 {
      font-size: 2rem;
      margin-bottom: 20px;
    }

    .about p {
      font-size: 1.1rem;
      line-height: 1.6;
    }

    footer {
      text-align: center;
      color: var(--cinza-medio);
      font-size: 0.9rem;
      margin-top: 40px;
      padding-bottom: 60px;
    }

    .slogan {
      font-weight: bold;
      color: var(--cinza-escuro);
      margin-top: 10px;
      font-size: 1rem;
      text-transform: uppercase;
    }

    .whatsapp-float {
      position: fixed;
      bottom: 20px;
      right: 20px;
      z-index: 999;
    }

    .whatsapp-float a {
      background-color: #25d366;
      color: white;
      border-radius: 50%;
      padding: 16px;
      text-align: center;
      display: inline-block;
      box-shadow: 0 4px 10px rgba(0,0,0,0.3);
      transition: transform 0.3s ease;
    }

    .whatsapp-float a:hover {
      transform: scale(1.1);
    }

    .whatsapp-float svg {
      width: 28px;
      height: 28px;
      fill: white;
    }

    @media (max-width: 768px) {
      .hero h1 {
        font-size: 2rem;
      }
      .benefits {
        flex-direction: column;
        align-items: center;
      }
    }
  </style>
  <script>
  function redirecionarParaEbook() {
    alert("Muito obrigado por baixar o eBook! Você será redirecionado agora.");
  }
</script>
</head>
<body>
  <div class="wrapper">
    <div class="logo">LÚCIO MEIRELES | ARQUITETO E URBANISTA</div>
    <section class="hero">
      <h1>AUMENTE ATÉ <span>40%</span> SUAS VENDAS COM ILUMINAÇÃO ESTRATÉGICA</h1>
      <p>Revelado: as estratégias de iluminação que lojas de luxo escondem para criar desejo imediato nos clientes – guia gratuito para você copiar!</p>
      <button class="btn" onclick="document.getElementById('form').scrollIntoView({behavior: 'smooth'})">QUERO MEU EBOOK GRÁTIS</button>
    </section>

    <section class="benefits">
      <div class="benefit">Técnicas validadas por Harvard e MIT</div>
      <div class="benefit">Caso real: +28% em vendas premium (em 30 dias)</div>
      <div class="benefit">Aplicável para lojas, restaurantes e escritórios</div>
    </section>

    <section class="form-section" id="form">
      <form action="https://formspree.io/f/xdkgypea" method="POST" onsubmit="setTimeout(function() { window.location.href = 'https://drive.google.com/file/d/1Jp_HoyRZSsiqpKTw3eQazdcdyxyvSmvv/view?usp=drive_link'; }, 1000); return true;">
        <input type="text" name="nome" placeholder="Seu nome" required>
        <input type="email" name="email" placeholder="Seu e-mail" required>
        <select name="segmento" required>
          <option disabled selected>Qual é o segmento do seu negócio?</option>
          <option value="moda">Moda</option>
          <option value="beleza">Beleza e Estética</option>
          <option value="saude">Saúde</option>
          <option value="alimentacao">Alimentação</option>
          <option value="academia">Academia</option>
          <option value="servicos">Serviços</option>
          <option value="varejo">Varejo em geral</option>
          <option value="escritório">Escritório</option>
        </select>
        <button class="btn" type="submit">RECEBER EBOOK</button>
      </form>
    </section>

    <!-- Restante da página permanece igual -->

    <div class="testimonial">"Apliquei as dicas do ebook e clientes elogiaram a 'nova atmosfera' da loja!" – Ana L., Boutique de Luxo</div>
    <div class="testimonial">"As estratégias de iluminação realmente aumentaram meu faturamento. Meu restaurante agora é mais acolhedor e moderno." – Carlos F., Restaurante Central</div>
    <div class="testimonial">"Em menos de um mês, senti o impacto nas vendas e na permanência dos clientes. Vale cada dica!" – Beatriz M., Loja de Calçados</div>
    <div class="testimonial">"Transformou totalmente nosso consultório. A iluminação trouxe uma sensação de sofisticação e conforto para os pacientes." – Dr. Renato A., Clínica Premium</div>

    <section class="about">
      <h2>Sobre Lúcio Meireles</h2>
      <p>Sou arquiteto e urbanista com mais de 5 anos de experiência no mercado de arquitetura comercial de alto padrão. Nos últimos anos, venho me especializando em lighting design, transformando espaços sem vida em verdadeiros ímãs de clientes. Acredito que uma boa iluminação é capaz de gerar mais conforto, valor percebido e aumento direto nas vendas.</p>
    </section>

    <footer>
      📞 (96) 98403-4253 | ✉ jluciosegundo@gmail.com<br>
      <div class="slogan">EXCELÊNCIA PARA QUEM EXIGE O EXTRAORDINÁRIO</div>
    </footer>
  </div>

  <div class="whatsapp-float">
    <a href="https://wa.me/message/C3WXQ4EL7UYBF1" target="_blank" aria-label="Fale conosco pelo WhatsApp">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32"><path d="M19.11 17.473c-.275-.138-1.626-.8-1.878-.89-.252-.093-.437-.138-.623.137-.184.275-.714.89-.876 1.073-.162.184-.323.207-.598.07-.275-.138-1.162-.428-2.212-1.362-.818-.73-1.37-1.63-1.53-1.904-.162-.275-.017-.424.122-.562.126-.125.275-.322.413-.483.138-.162.184-.275.275-.46.092-.184.046-.345-.023-.483-.068-.138-.622-1.5-.852-2.05-.224-.538-.452-.464-.622-.472-.16-.006-.344-.008-.53-.008-.183 0-.48.07-.732.345-.253.275-.964.94-.964 2.29 0 1.351.986 2.653 1.122 2.837.137.184 1.94 2.963 4.694 4.15.657.283 1.17.452 1.57.577.66.21 1.26.18 1.733.11.529-.08 1.626-.663 1.857-1.305.23-.644.23-1.194.16-1.305-.068-.11-.252-.184-.528-.322m-3.11 9.848c-1.285 0-2.542-.208-3.724-.617l-4.15.61.652-4.044c-.829-1.145-1.456-2.41-1.857-3.76-.407-1.358-.612-2.766-.61-4.187.007-2.354.704-4.645 2.008-6.596C9.548 5.78 10.65 4.784 11.9 4.05c1.251-.732 2.654-1.12 4.11-1.118h.01c4.198 0 7.682 2.77 8.907 6.764 1.14 3.685.103 7.637-2.705 10.354-1.692 1.66-3.91 2.653-6.212 2.893-.59.063-1.184.095-1.777.095m7.467-17.305C21.875 6.072 19.32 4.51 16.374 4.51h-.01c-1.195 0-2.354.322-3.377.935-.94.55-1.747 1.312-2.37 2.237-1.047 1.527-1.6 3.32-1.607 5.165-.002 1.24.19 2.468.573 3.65.384 1.282 1.017 2.475 1.86 3.53l-.384 2.38 2.45-.36c1.02.528 2.107.892 3.234 1.084 2.038.325 4.154-.23 5.81-1.542 2.398-2.134 3.305-5.47 2.373-8.525-.877-2.84-2.708-4.887-5.156-5.969"/></svg>
    </a>
  </div>
</body>
</html>
