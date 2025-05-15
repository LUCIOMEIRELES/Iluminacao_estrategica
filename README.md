<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Iluminação Estratégica – Aumente suas vendas</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&display=swap');

  :root {
    --cinza-escuro: #3A4550;
    --cinza-medio: #7E8C97;
    --cinza-claro: #B1B9C1;
    --cinza-claro-textura: #e5e5e5;
    --branco: #DDE1E6;
    --btn-bg: #7E8C97;
    --btn-bg-hover: #6a7886;
  }

  * {
    box-sizing: border-box;
  }

  body {
    margin: 0;
    font-family: 'Montserrat', sans-serif;
    background: var(--cinza-claro-textura);
    color: var(--cinza-escuro);
  }

  /* Textura sutil de concreto claro */
  body::before {
    content: "";
    position: fixed;
    top: 0; left: 0; right: 0; bottom: 0;
    background: url('https://www.transparenttextures.com/patterns/concrete-texture.png') repeat;
    opacity: 0.08;
    pointer-events: none;
    z-index: -1;
  }

  .container {
    max-width: 480px;
    margin: 40px auto 80px;
    background: var(--branco);
    border-radius: 24px;
    box-shadow: 0 10px 40px rgba(0,0,0,0.1);
    overflow: hidden;
  }

  header {
    background: var(--cinza-escuro);
    color: var(--branco);
    padding: 24px 30px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 600;
    letter-spacing: 4px;
    font-size: 1.15rem;
    font-feature-settings: "liga", "clig";
    user-select: none;
  }

  /* Hero section */
  .hero {
    padding: 48px 30px 60px;
    text-align: center;
    position: relative;
  }

  .hero h1 {
    font-weight: 700;
    font-size: 2.2rem;
    margin: 0 0 16px;
    letter-spacing: 2px;
    color: var(--cinza-escuro);
  }

  .hero h1 span {
    color: var(--cinza-medio);
  }

  .hero p {
    font-weight: 400;
    font-size: 1.05rem;
    margin: 0 0 36px;
    color: var(--cinza-medio);
  }

  /* Botão CTA cinza */
  .btn-cta {
    background-color: var(--btn-bg);
    color: var(--cinza-claro);
    font-weight: 700;
    font-size: 1.2rem;
    padding: 16px 30px;
    border-radius: 30px;
    border: none;
    cursor: pointer;
    box-shadow: 0 5px 0 var(--cinza-escuro);
    transition: background-color 0.3s ease, transform 0.2s ease;
    display: inline-flex;
    align-items: center;
    gap: 12px;
    user-select: none;
  }
  .btn-cta:hover {
    background-color: var(--btn-bg-hover);
    transform: translateY(-3px);
  }
  .btn-cta:active {
    transform: translateY(0);
    box-shadow: none;
  }

  /* Ícone download */
  .btn-cta svg {
    width: 22px;
    height: 22px;
    fill: var(--cinza-claro);
  }

  /* Benefícios */
  .benefits {
    background: var(--cinza-escuro);
    color: var(--branco);
    padding: 40px 30px;
    border-radius: 0 0 24px 24px;
    margin-top: -48px;
    box-shadow: 0 10px 25px rgba(58,69,80,0.2);
  }

  .benefits ul {
    list-style: none;
    padding: 0;
    margin: 0;
  }

  .benefits li {
    display: flex;
    align-items: center;
    font-weight: 500;
    font-size: 1rem;
    margin-bottom: 20px;
    gap: 16px;
  }

  .benefits li:last-child {
    margin-bottom: 0;
  }

  .benefits li svg {
    width: 22px;
    height: 22px;
    fill: var(--cinza-medio);
    flex-shrink: 0;
  }

  /* Formulário */
  form {
    margin: 40px 30px 60px;
    display: flex;
    flex-direction: column;
    gap: 24px;
  }

  input, select {
    padding: 14px 20px;
    border-radius: 12px;
    border: 2px solid var(--cinza-claro);
    font-size: 1rem;
    font-weight: 600;
    color: var(--cinza-escuro);
    transition: border-color 0.3s ease;
  }

  input::placeholder,
  select option:first-child {
    color: var(--cinza-medio);
    font-weight: 400;
  }

  input:focus, select:focus {
    outline: none;
    border-color: var(--cinza-medio);
    box-shadow: 0 0 8px #7e8c9755;
  }

  /* Botão enviar do formulário */
  button[type="submit"] {
    background-color: var(--btn-bg);
    color: var(--cinza-claro);
    font-weight: 700;
    font-size: 1.15rem;
    padding: 16px 0;
    border-radius: 30px;
    border: none;
    cursor: pointer;
    box-shadow: 0 5px 0 var(--cinza-escuro);
    transition: background-color 0.3s ease, transform 0.2s ease;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 12px;
    user-select: none;
  }
  button[type="submit"]:hover {
    background-color: var(--btn-bg-hover);
    transform: translateY(-3px);
  }
  button[type="submit"]:active {
    transform: translateY(0);
    box-shadow: none;
  }
  button[type="submit"] svg {
    width: 22px;
    height: 22px;
    fill: var(--cinza-claro);
  }

  /* Prova social */
  .testimonial {
    background: var(--cinza-claro);
    color: var(--cinza-escuro);
    font-style: italic;
    font-weight: 500;
    margin: 0 30px 60px;
    padding: 24px 30px;
    border-radius: 20px;
    box-shadow: 0 10px 25px rgba(0,0,0,0.08);
    position: relative;
    font-size: 1rem;
    user-select: none;
  }

  .testimonial::before {
    content: "“";
    font-size: 3rem;
    color: var(--cinza-medio);
    position: absolute;
    top: 15px;
    left: 20px;
    opacity: 0.3;
    font-weight: 700;
    user-select: none;
  }

  /* Rodapé */
  footer {
    text-align: center;
    padding: 24px 20px;
    font-size: 0.9rem;
    color: var(--cinza-medio);
    user-select: none;
  }

  footer .contact {
    margin-bottom: 8px;
  }

  footer .selo {
    font-weight: 700;
    color: var(--cinza-escuro);
  }

  /* Responsividade */
  @media (max-width: 520px) {
    .container {
      margin: 20px 15px 50px;
    }
    .hero h1 {
      font-size: 1.8rem;
      letter-spacing: 1.5px;
    }
    .benefits {
      padding: 30px 20px;
    }
    form {
      margin: 30px 20px 50px;
      gap: 18px;
    }
    .testimonial {
      margin: 0 20px 50px;
      font-size: 0.95rem;
      padding: 20px 20px;
    }
  }
</style>
</head>
<body>

  <div class="container" role="main" aria-label="Landing page para captação do ebook Iluminação Estratégica">

    <header aria-label="Logotipo Lúcio Meireles Arquiteto e Urbanista">
      LÚCIO MEIRELES | ARQUITETO E URBANISTA
    </header>

    <section class="hero" aria-label="Seção principal com chamada para baixar ebook">
      <h1>AUMENTE ATÉ <span>40%</span> SUAS VENDAS COM ILUMINAÇÃO ESTRATÉGICA</h1>
      <p>Baixe o ebook gratuito e descubra técnicas usadas por lojas premium</p>
      <button class="btn-cta" onclick="document.getElementById('form-captura').scrollIntoView({behavior:'smooth'})" aria-label="Ir para formulário para receber ebook">
        QUERO MEU EBOOK GRÁTIS
        <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false"><path d="M12 16l4-5h-3V4h-2v7H8l4 5z"></path></svg>
      </button>
    </section>

    <section class="benefits" aria-label="Benefícios do ebook">
      <ul>
        <li>
          <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false"><path d="M9 16.172l-3.586-3.586-1.414 1.414L9 19 20 8l-1.414-1.414z"/></svg>
          Técnicas validadas por Harvard e MIT
        </li>
        <li>
          <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false"><path d="M9 16.172l-3.586-3.586-1.414 1.414L9 19 20 8l-1.414-1.414z"/></svg>
          Caso real: +28% em vendas premium (em 30 dias)
        </li>
        <li>
          <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false"><path d="M9 16.172l-3.586-3.586-1.414 1.414L9 19 20 8l-1.414-1.414z"/></svg>
          Aplicável para lojas, restaurantes e escritórios
        </li>
      </ul>
    </section>

    <form id="form-captura" action="https://formspree.io/f/xdkgypea" method="POST" onsubmit="enviar(event)" novalidate aria-label="Formulário para captação de leads">
      <input type="text" name="nome" placeholder="Seu nome" required aria-required="true" />
      <input type="email" name="email" placeholder="Seu e-mail" required aria-required="true" />
      <select name="segmento" required aria-required="true" aria-label="Selecione o segmento do seu negócio">
        <option value="" disabled selected>Qual é o segmento do seu negócio?</option>
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
      <button type="submit" aria-label="Enviar formulário para receber o eBook">
        RECEBER EBOOK GRÁTIS
        <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false"><path d="M12 16l4-5h-3V4h-2v7H8l4 5z"></path></svg>
      </button>
    </form>

    <section class="testimonial" aria-label="Depoimento de cliente satisfeito">
      "Apliquei as dicas do ebook e clientes elogiaram a 'nova atmosfera' da loja!" – Ana L., Boutique de Luxo
    </section>

    <footer>
      <div class="contact" aria-label="Contato do escritório">
        📞 (96) 98403-4253 | ✉ jluciosegundo@gmail.com
      </div>
      <div class="selo" aria-label="Selo de arquitetura comercial especializada">
        ARQUITETURA COMERCIAL ESPECIALIZADA
      </div>
    </footer>

  </div>

<script>
  function enviar(e) {
    e.preventDefault();
    const form = e.target;
    const data = new FormData(form);

    fetch(form.action, {
      method: 'POST',
      body: data,
      headers: { 'Accept': 'application/json' }
    }).then(response => {
      if (response.ok) {
        alert('Enviado com sucesso! Você será redirecionado para o download do eBook.');
        window.location.href = 'https://drive.google.com/file/d/1Jp_HoyRZSsiqpKTw3eQazdcdyxyvSmvv/view?usp=drive_link';
      } else {
        alert('Erro ao enviar. Por favor, tente novamente.');
      }
    });
  }
</script>

</body>
</html>
