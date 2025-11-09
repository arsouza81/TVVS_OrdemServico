<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Manual – Sistema Ordem de Serviços</title>
  <style>
    :root {
      --sidebar-width: 280px;
      --accent: #0d6efd;
      --text: #000;
      --muted: #555;
      --border: #ccc;
    }

    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body { margin: 0; font: 16px/1.6 system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, Noto Sans, sans-serif; color: var(--text); background: #fff; }

    /* ===== Sidebar ===== */
    .layout { display: flex; min-height: 100vh; }

    .sidebar {
      position: fixed; inset: 0 auto 0 0; width: var(--sidebar-width);
      background: #f5f5f5;
      border-right: 1px solid var(--border);
      padding: 18px 16px 24px; overflow-y: auto; z-index: 20;
    }

    .brand { display: flex; align-items: center; gap: 10px; margin: 4px 0 14px; }
    .brand .logo { width: 40px; height: 40px; border-radius: 8px; object-fit: contain; }
    .brand h1 { font-size: 15px; margin: 0; letter-spacing: .2px; color: var(--text); }

    .search { position: sticky; top: 0; padding-bottom: 10px; background: #f5f5f5; }
    .search input {
      width: 100%; padding: 10px 12px; border-radius: 10px; border: 1px solid var(--border);
      background: #fff; color: var(--text);
    }

    nav { margin-top: 12px; }
    .group-title { font-size: 11px; text-transform: uppercase; letter-spacing: .12em; color: var(--muted); margin: 16px 10px 6px; }
    .menu { list-style: none; margin: 0; padding: 0; }
    .menu a {
      display: block; padding: 9px 12px; margin: 4px 6px; border-radius: 10px; text-decoration: none;
      color: var(--text); border: 1px solid transparent; transition: .18s ease;
    }
    .menu a:hover { background: #e9ecef; border-color: #ccc; }
    .menu a.active { background: #dbeafe; border-color: #a7c7f9; color: #0d6efd; }

    /* ===== Content ===== */
    .content {
      margin-left: var(--sidebar-width); width: calc(100% - var(--sidebar-width));
      padding: 32px 9vw; max-width: 1100px;
    }

    header.topbar { position: sticky; top: 0; z-index: 10; background: #fff; border-bottom: 1px solid var(--border); margin: -32px -9vw 24px; padding: 14px 9vw; }
    header .title { font-size: 20px; font-weight: 650; }

    section { scroll-margin-top: 76px; }
    .card { background: #fff; border: 1px solid var(--border); border-radius: 16px; padding: 22px; box-shadow: 0 4px 10px rgba(0,0,0,.05); }

    h2 { font-size: 26px; margin: 0 0 8px; color: var(--text); }
    h3 { font-size: 18px; margin: 18px 0 8px; color: var(--text); }
    p, li { color: var(--text); }
    code, pre { background: #f8f9fa; color: #000; border: 1px solid #ccc; border-radius: 10px; }
    code { padding: 2px 6px; }
    pre { padding: 14px; overflow: auto; }

    .kbd { display: inline-block; border: 1px solid #ccc; background: #f8f9fa; padding: 1px 6px; border-radius: 6px; font-size: .9em; }
    .note { border-left: 3px solid var(--accent); padding-left: 10px; color: var(--text); }

    footer { margin: 40px 0 80px; color: var(--muted); font-size: 14px; }
    .back-to-top { position: fixed; right: 22px; bottom: 22px; padding: 10px 12px; border-radius: 12px; border: 1px solid var(--border); background: #fff; color: var(--text); text-decoration: none; }

    /* ===== Responsive ===== */
    .mobile-toggle { display: none; position: fixed; left: 12px; top: 12px; z-index: 30; }
    .mobile-toggle button { padding: 8px 10px; border-radius: 10px; border: 1px solid var(--border); background: #fff; color: var(--text); }

    @media (max-width: 980px) {
      :root { --sidebar-width: 242px; }
      .content { padding: 28px 6vw; margin-left: 0; width: 100%; }
      .sidebar { transform: translateX(-100%); transition: transform .25s ease; }
      .sidebar.open { transform: translateX(0); }
      .mobile-toggle { display: block; }
      header.topbar { padding-left: calc(6vw + 48px); }
      section { scroll-margin-top: 92px; }
    }
  </style>
</head>
<body>
  <div class="layout">
    <!-- Sidebar -->
    <aside class="sidebar" id="sidebar">
      <div class="brand">
        <img src="imagens/logo.png" alt="Logo do sistema" class="logo">
        <h1>Ordem de Serviço</h1>
      </div>

      <div class="search">
        <input id="filter" type="search" placeholder="Filtrar seções (Ctrl+/)" aria-label="Filtrar seções" />
      </div>

      <nav aria-label="Navegação do manual">
        <div class="group">
          <div class="group-title">Guia</div>
          <ul class="menu" id="menu">
            <li><a href="#intro">Introdução</a></li>
            <li><a href="#instalacao">Instalação</a></li>
            <li><a href="#config">Configuração</a></li>
            <li><a href="#uso">Uso Básico</a></li>
            <li><a href="#funcionalidades">Funcionalidades</a></li>
            <li><a href="#dicas">Boas Práticas</a></li>
            <li><a href="#faq">Perguntas Frequentes</a></li>
            <li><a href="#suporte">Suporte</a></li>
          </ul>
        </div>
      </nav>
    </aside>

    <!-- Content -->
    <main class="content" id="conteudo">
      <div class="mobile-toggle">
        <button id="toggleNav" aria-expanded="false" aria-controls="sidebar">Menu</button>
      </div>

      <header class="topbar">
        <div class="title">Manual do Sistema Ordem de Serviço - OS</div>
      </header>

      <section id="intro" class="card" aria-labelledby="h-intro">
        <h2 id="h-intro">Introdução</h2>
        <p>Bem-vindo ao manual do Sistema <strong>Ordem de Serviços</strong>. Este documento descreve os passos essenciais para instalação, configuração e uso do sistema. Use o menu à esquerda como âncora para navegar rapidamente entre as seções.</p>
        <p class="note">Dica: pressione <span class="kbd">Ctrl</span> + <span class="kbd">/</span> para focar o campo de filtro e localizar uma seção.</p>
      </section>

      <section id="instalacao" class="card" aria-labelledby="h-instalacao" style="margin-top: 26px;">
        <h2 id="h-instalacao">Instalação</h2>
        <h3>Requisitos</h3>
        <ul>
          <li>Sistema operacional compatível (Windows, macOS, Linux)</li>
          <li>Permissões administrativas</li>
          <li>Conexão à internet</li>
        </ul>
        <h3>Passos</h3>
        <ol>
          <li>Baixe o instalador no portal oficial.</li>
          <li>Execute o instalador e siga as instruções exibidas.</li>
          <li>Finalize e reinicie a aplicação, se necessário.</li>
        </ol>
        <pre><code># Exemplo via linha de comando (Linux)
sudo dpkg -i produto_amd64.deb
sudo apt-get -f install</code></pre>
      </section>

      <section id="config" class="card" aria-labelledby="h-config" style="margin-top: 26px;">
        <h2 id="h-config">Configuração</h2>
        <p>Após instalar, ajuste os parâmetros em <code>config.yaml</code>:</p>
        <pre><code>servidor:
  host: 0.0.0.0
  porta: 8080
seguranca:
  modo: "producao"
  jwt_secret: "altere-esta-chave"
log:
  nivel: "info"</code></pre>
        <p>Salve o arquivo e reinicie o serviço.</p>
      </section>

      <section id="uso" class="card" aria-labelledby="h-uso" style="margin-top: 26px;">
        <h2 id="h-uso">Uso Básico</h2>
        <ol>
          <li>Abra o aplicativo e realize login.</li>
          <li>Acesse o menu <em>Painel</em> para visão geral.</li>
          <li>Utilize as abas para navegar entre módulos.</li>
        </ol>
        <p class="note">Observação: recursos podem variar conforme permissões do usuário.</p>
      </section>

      <section id="funcionalidades" class="card" aria-labelledby="h-atalhos" style="margin-top: 26px;">
        <h2 id="h-atalhos">Funcionalidades</h2>
        <ul>
          <li><span class="kbd">Ctrl</span> + <span class="kbd">K</span> — Busca global</li>
          <li><span class="kbd">?</span> — Ajuda</li>
          <li><span class="kbd">G</span> depois <span class="kbd">D</span> — Ir para Dashboard</li>
        </ul>
      </section>

      <section id="dicas" class="card" aria-labelledby="h-dicas" style="margin-top: 26px;">
        <h2 id="h-dicas">Boas Práticas</h2>
        <ul>
          <li>Mantenha o sistema atualizado.</li>
          <li>Use senhas fortes e ative MFA.</li>
          <li>Faça backup regular dos dados.</li>
        </ul>
      </section>

      <section id="faq" class="card" aria-labelledby="h-faq" style="margin-top: 26px;">
        <h2 id="h-faq">Perguntas Frequentes (FAQ)</h2>
        <h3>Como redefinir a senha?</h3>
        <p>No menu de login, clique em <em>Esqueci minha senha</em> e siga as instruções enviadas por e-mail.</p>
        <h3>Como atualizar?</h3>
        <p>Abra <em>Configurações &gt; Atualizações</em> e verifique se há uma nova versão disponível.</p>
      </section>

      <section id="suporte" class="card" aria-labelledby="h-suporte" style="margin-top: 26px;">
        <h2 id="h-suporte">Suporte</h2>
        <p>Se precisar de ajuda adicional, contate a equipe responsável ou abra um chamado no sistema de suporte.</p>
      </section>

      <footer>
        © <span id="year"></span> – Manual do Sistema Ordem de Serviços. Todos os direitos reservados.
      </footer>
    </main>
  </div>

  <a href="#intro" class="back-to-top" aria-label="Voltar ao topo">↑ Topo</a>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();

    const sidebar = document.getElementById('sidebar');
    const toggleNav = document.getElementById('toggleNav');
    toggleNav?.addEventListener('click', () => {
      const open = sidebar.classList.toggle('open');
      toggleNav.setAttribute('aria-expanded', String(open));
    });

    const filter = document.getElementById('filter');
    const menu = document.getElementById('menu');
    const items = [...menu.querySelectorAll('li')];

    document.addEventListener('keydown', (e) => {
      if ((e.ctrlKey || e.metaKey) && e.key === '/') {
        e.preventDefault();
        filter.focus();
      }
    });

    filter.addEventListener('input', () => {
      const q = filter.value.trim().toLowerCase();
      items.forEach(li => {
        const text = li.textContent.toLowerCase();
        li.style.display = text.includes(q) ? '' : 'none';
      });
    });

    const links = [...document.querySelectorAll('.menu a')];
    const sections = links.map(a => document.querySelector(a.getAttribute('href')));

    const activate = (id) => {
      links.forEach(a => a.classList.toggle('active', a.getAttribute('href') === `#${id}`));
    };

    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) activate(entry.target.id);
      });
    }, { rootMargin: '-60% 0px -35% 0px', threshold: 0.01 });

    sections.forEach(sec => sec && observer.observe(sec));

    links.forEach(a => a.addEventListener('click', () => {
      if (window.matchMedia('(max-width: 980px)').matches) sidebar.classList.remove('open');
    }));
  </script>
</body>
</html>
