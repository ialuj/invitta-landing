<template>
  <div class="landing">
    <header>
      <img src="/images/logo.png" alt="Invitta Logo" class="logo" />
      <p class="tagline">Convide. Organize. Celebre.</p>
      <button @click="scrollToSection('about')">Saiba mais</button>
    </header>

    <main>
      <section id="about">
        <h2>O que é o Invitta?</h2>
        <p>
          O <strong>Invitta</strong> é uma plataforma inteligente para a gestão
          de convites de eventos como casamentos, aniversários, noivados,
          jantares de gala, conferências e muito mais. Ele permite que
          organizadores criem eventos com facilidade, enviem convites digitais,
          recebam confirmações e acompanhem todos os detalhes com praticidade.
        </p>
      </section>

      <section id="mvp">
        <h2>MVP: O que esperamos entregar</h2>
        <ul>
          <li>🔐 Login via número de telefone</li>
          <li>🎉 Criação e personalização de eventos</li>
          <li>
            📱 Cadastro de convidados e envio de convites em PDF via WhatsApp
          </li>
          <li>✅ Confirmação de presença (RSVP)</li>
          <li>🍽️ Definição de mesas e preferências alimentares</li>
          <li>👀 Acesso simplificado ao app pelos convidados</li>
        </ul>
      </section>

      <section id="future">
        <h2>Recursos futuros</h2>
        <ul>
          <li>📊 Painel avançado com estatísticas do evento</li>
          <li>🧾 Check-in por QR code no local</li>
          <li>🔔 Notificações automáticas para convidados</li>
          <li>🎨 Temas personalizados para o evento</li>
          <li>🧑‍🍳 Modo garçom com visualização de mesas e restrições</li>
          <li>🌐 Tradução multilíngue automático</li>
        </ul>
      </section>

      <section id="download">
        <h2>Como baixar</h2>
        <p>O app estará disponível em breve nas principais plataformas:</p>
        <div class="store-links">
          <a href="https://play.google.com/store" target="_blank">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg"
              alt="Google Play"
            />
          </a>
          <a href="https://www.apple.com/app-store/" target="_blank">
            <img src="/images/apple.svg" alt="App Store" />
          </a>
        </div>
      </section>
    </main>

    <footer>
      <p>Desenvolvido por <strong>Phanda Tech Solutions, SU, LDA</strong> ·</p>
      <p><a href="mailto:info@phandatech.com">info@phandatech.com</a><br /></p>
      <p>
        <a href="https://ialuj.github.io/phanda-site/" target="_blank"
          >www.phandatech.com</a
        >
      </p>
      <p><small>&copy; 2025 Invitta. Todos os direitos reservados.</small></p>
    </footer>
  </div>
</template>

<script setup>
const scrollToSection = (id) => {
  const el = document.getElementById(id);
  if (el) el.scrollIntoView({ behavior: "smooth" });
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html,
body,
.landing {
  height: 100%;
  width: 100%;
}

body {
  font-family: "Poppins", sans-serif;
  background-color: #f9fafb;
  color: #333;
}

.landing {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

header {
  text-align: center;
  padding: 4rem 1rem 3rem;
  background-color: #6c63ff;
  color: white;
}

.logo {
  height: 150px;
  margin-bottom: 1rem;
}

.tagline {
  font-size: 1.25rem;
  margin-bottom: 1.5rem;
}

button {
  background-color: #4ade80;
  border: none;
  color: white;
  font-weight: bold;
  padding: 0.75rem 1.5rem;
  border-radius: 6px;
  cursor: pointer;
}

main {
  flex: 1;
  padding: 2rem 1rem;
}

section {
  max-width: 800px;
  margin: 3rem auto;
}

section h2 {
  font-size: 1.75rem;
  margin-bottom: 1rem;
  color: #6c63ff;
}

ul {
  list-style-type: none;
  padding: 0;
}

ul li {
  margin: 0.5rem 0;
  font-size: 1rem;
}

.store-links {
  display: flex;
  gap: 1rem;
  justify-content: center;
  margin-top: 1rem;
}

.store-links img {
  height: 48px;
}

footer {
  background-color: #f4f4f4;
  text-align: center;
  font-size: 0.875rem;
  padding: 2rem 1rem;
  color: #666;
}

footer a {
  color: #6c63ff;
  text-decoration: none;
}
</style>
