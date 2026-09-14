---
title: HortPay
---

<style>
:root {
  --green: #2E7D32;
  --green-light: #5E8F3B;
  --green-soft: #E7F0D8;
  --dark: #17321A;
  --text: #46534A;
  --white: #FFFFFF;
}

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Arial, sans-serif;
  color: var(--text);
  background: #F7F9F5;
}

.hp-hero {
  background: linear-gradient(135deg, #1B5E20 0%, #2E7D32 45%, #5E8F3B 100%);
  color: white;
  text-align: center;
  padding: 85px 25px 80px;
  margin: -20px -20px 55px;
  border-radius: 0 0 28px 28px;
  box-shadow: 0 8px 30px rgba(46, 125, 50, 0.18);
}

.hp-logo {
  font-size: 52px;
  margin-bottom: 16px;
  filter: drop-shadow(0 2px 4px rgba(0,0,0,0.15));
}

.hp-hero h1 {
  font-size: 50px;
  margin: 0 0 14px;
  font-weight: 800;
  letter-spacing: -1.2px;
  text-shadow: 0 2px 4px rgba(0,0,0,0.12);
}

.hp-hero p {
  font-size: 18px;
  max-width: 680px;
  margin: 0 auto;
  opacity: .92;
  line-height: 1.7;
  font-weight: 400;
  letter-spacing: .1px;
}

.hp-badge {
  display: inline-flex;
  align-items: center;
  margin-top: 28px;
  padding: 10px 18px;
  border: 1px solid rgba(255,255,255,.28);
  border-radius: 999px;
  background: rgba(255,255,255,.08);
  backdrop-filter: blur(8px);
  font-size: 13px;
  font-weight: 500;
  letter-spacing: .2px;
}

.hp-container {
  max-width: 1050px;
  margin: auto;
  padding: 0 20px 50px;
}

.hp-intro {
  text-align: center;
  max-width: 800px;
  margin: 0 auto 55px;
}

.hp-intro h2 {
  color: var(--dark);
  font-size: 32px;
  margin-bottom: 15px;
}

.hp-intro p {
  font-size: 18px;
  line-height: 1.7;
}

.hp-section-title {
  text-align: center;
  color: var(--dark);
  font-size: 30px;
  margin: 55px 0 25px;
}

.hp-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.hp-card {
  background: white;
  border: 1px solid #E2E9DF;
  border-radius: 16px;
  padding: 25px;
  box-shadow: 0 5px 18px rgba(30,60,30,.06);
}

.hp-card-icon {
  font-size: 32px;
  margin-bottom: 12px;
}

.hp-card h3 {
  color: var(--green);
  margin: 0 0 10px;
  font-size: 19px;
}

.hp-card p {
  margin: 0;
  line-height: 1.6;
  font-size: 15px;
}

.hp-highlight {
  background: linear-gradient(135deg, #E7F0D8, #F4F8EF);
  border-radius: 20px;
  padding: 38px;
  margin-top: 45px;
  text-align: center;
  border: 1px solid #D6E4CA;
}

.hp-highlight h2 {
  color: var(--dark);
  margin-top: 0;
  font-size: 28px;
}

.hp-highlight p {
  max-width: 720px;
  margin: auto;
  line-height: 1.7;
  font-size: 17px;
}

.hp-links {
  text-align: center;
  margin-top: 55px;
  padding-top: 35px;
  border-top: 1px solid #DDE5DA;
}

.hp-links a {
  color: var(--green);
  font-weight: 600;
  text-decoration: none;
  margin: 0 14px;
}

.hp-links a:hover {
  text-decoration: underline;
}

.hp-footer {
  text-align: center;
  margin-top: 35px;
  color: #7B857D;
  font-size: 14px;
}

@media (max-width: 750px) {
  .hp-hero h1 {
    font-size: 40px;
  }

  .hp-hero p {
    font-size: 18px;
  }

  .hp-grid {
    grid-template-columns: 1fr;
  }

  .hp-intro h2 {
    font-size: 27px;
  }

  .hp-highlight {
    padding: 28px 20px;
  }

  .hp-links a {
    display: block;
    margin: 15px 0;
  }
}
  .hp-hero-image {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto 35px;
  text-align: center;
}

.hp-hero-image img {
  width: 100%;
  height: auto;
  display: block;
  border-radius: 0 0 24px 24px;
}
</style>

<div class="hp-hero-image">
  <img src="hortpay-site.png" alt="HortPay — Gestão agrícola">
</div>

<div class="hp-container">

  <div class="hp-intro">
    <h2>Mais controle para sua propriedade rural</h2>

    <p>
      O <strong>HortPay</strong> é um aplicativo desenvolvido para facilitar
      o gerenciamento da propriedade rural, permitindo controlar produção,
      vendas, estoque, custos e atividades agrícolas diretamente pelo celular.
    </p>
  </div>

  <h2 class="hp-section-title">Tudo em um só lugar</h2>

  <div class="hp-grid">

    <div class="hp-card">
      <div class="hp-card-icon">💰</div>
      <h3>Controle financeiro</h3>
      <p>
        Registre vendas, despesas, contas a pagar e receber e acompanhe
        a movimentação financeira da propriedade.
      </p>
    </div>

    <div class="hp-card">
      <div class="hp-card-icon">🌱</div>
      <h3>Gestão de cultivos</h3>
      <p>
        Organize seus cultivos, ciclos de produção, estufas e atividades
        realizadas durante o desenvolvimento das plantas.
      </p>
    </div>

    <div class="hp-card">
      <div class="hp-card-icon">📦</div>
      <h3>Controle de estoque</h3>
      <p>
        Controle produtos, insumos, quantidades, preços e movimentações
        de estoque.
      </p>
    </div>

    <div class="hp-card">
      <div class="hp-card-icon">💧</div>
      <h3>Fertirrigação</h3>
      <p>
        Registre aplicações, produtos utilizados, dosagens e informações
        importantes do manejo nutricional.
      </p>
    </div>

    <div class="hp-card">
      <div class="hp-card-icon">🍃</div>
      <h3>Aplicações foliares</h3>
      <p>
        Organize aplicações foliares e acompanhe produtos, doses e custos
        das operações realizadas.
      </p>
    </div>

    <div class="hp-card">
      <div class="hp-card-icon">📊</div>
      <h3>Relatórios</h3>
      <p>
        Tenha uma visão organizada das informações da propriedade para
        acompanhar seus resultados.
      </p>
    </div>

  </div>

  <div class="hp-highlight">

    <h2>📱 Funciona mesmo sem internet</h2>

    <p>
      O HortPay foi desenvolvido com uma abordagem <strong>offline-first</strong>.
      Suas informações podem ser registradas diretamente no dispositivo,
      mesmo quando não houver conexão com a internet.
    </p>

    <p style="margin-top:18px;">
      Quando utilizado, o backup no <strong>Google Drive</strong> permite
      proteger seus dados e facilitar sua recuperação.
    </p>

  </div>

  <h2 class="hp-section-title">Por que escolher o HortPay?</h2>

  <div class="hp-grid">

    <div class="hp-card">
      <div class="hp-card-icon">📱</div>
      <h3>Feito para celular</h3>
      <p>
        Interface pensada para facilitar o uso durante a rotina no campo.
      </p>
    </div>

    <div class="hp-card">
      <div class="hp-card-icon">🌾</div>
      <h3>Focado na agricultura</h3>
      <p>
        Recursos desenvolvidos pensando nas necessidades da gestão rural.
      </p>
    </div>

    <div class="hp-card">
      <div class="hp-card-icon">🔒</div>
      <h3>Privacidade</h3>
      <p>
        Transparência sobre o tratamento das informações e utilização
        dos recursos do aplicativo.
      </p>
    </div>

  </div>

  <div class="hp-links">

    <a href="https://hortpay.app.br/privacy-policy.html">
      🔒 Política de Privacidade
    </a>

    <a href="https://hortpay.app.br/terms-of-service.html">
      📄 Termos de Serviço
    </a>

  </div>

  <div class="hp-footer">
    <strong>HortPay</strong> — Gestão financeira agrícola
    <br>
    © 2026 HortPay. Todos os direitos reservados.
  </div>

</div>
