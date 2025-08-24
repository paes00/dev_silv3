<!DOCTYPE html>
<html lang="pt-BR">
<head>  
  <meta charset="UTF-8">  
  <meta name="viewport" content="width=device-width, initial-scale=1.0">  
  <title>dev_silv - Segurança Digital</title>  
  <!-- Google Fonts -->  
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">  
  <!-- Font Awesome -->  
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">  
  <style>
  
    * { margin:0; padding:0; box-sizing:border-box; }
    html { scroll-behavior: smooth; }
    body { font-family:'Montserrat',sans-serif; background:#0d1117; color:#e6edf3; line-height:1.6; }

    /* ====== HEADER ====== */
    header { background:#161b22; padding:15px 20px; display:flex; justify-content:space-between; align-items:center; position:sticky; top:0; z-index:1000; box-shadow:0 2px 6px rgba(0,0,0,0.5); }
    header .logo { display:flex; align-items:center; gap:10px; }
    header h1 { font-size:1.5rem; color:#58a6ff; }
    nav ul { display:flex; gap:25px; list-style:none; }
    nav ul li a { color:#e6edf3; text-decoration:none; font-weight:600; transition: all 0.3s; }
    nav ul li a:hover { color:#58a6ff; transform:scale(1.05); }

    /* ====== SECTIONS ====== */
    section { padding:60px 20px; max-width:1000px; margin:auto; opacity:0; transform: translateY(40px); transition: all 1s ease; border-radius:15px; }
    section.visible { opacity:1; transform: translateY(0); }
    section:nth-child(even) { background: linear-gradient(135deg,#0d1117,#161b22); }
    section:nth-child(odd) { background: linear-gradient(135deg,#161b22,#1a202c); }
    h2 { font-size:2rem; margin-bottom:20px; color:#58a6ff; border-left:5px solid #58a6ff; padding-left:12px; }

    /* ====== CARDS ====== */
    .card { background:#1b222b; padding:25px; border-radius:15px; margin:20px 0; box-shadow:0 8px 20px rgba(0,0,0,0.5); transition: transform 0.3s ease, box-shadow 0.3s ease; }
    .card:hover { transform:translateY(-7px); box-shadow:0 12px 25px rgba(0,0,0,0.6); }
    ul { list-style:none; padding-left:0; }
    ul li { margin:12px 0; padding-left:30px; position:relative; font-size:1.05rem; }
    ul li::before { content:"\f00c"; font-family:"Font Awesome 6 Free"; font-weight:900; position:absolute; left:0; color:#3fb950; }
    iframe { width:100%; height:400px; border:none; border-radius:12px; }

    /* ====== BOTÕES ====== */
    a.button { display:inline-block; padding:12px 25px; background-color:#58a6ff; color:#fff; border-radius:10px; text-decoration:none; font-weight:600; transition: all 0.3s; }
    a.button:hover { background-color:#3b82f6; transform:translateY(-3px); }

    /* ====== BOTÃO VOLTAR AO TOPO ====== */
    #topBtn { position: fixed; bottom:30px; right:30px; display:none; z-index:100; background:#58a6ff; color:#fff; border:none; padding:12px 16px; border-radius:50%; cursor:pointer; font-size:20px; transition: background 0.3s; }
    #topBtn:hover { background:#3b82f6; }

    /* ====== FOOTER ====== */
    footer { background:#161b22; text-align:center; padding:20px; font-size:0.95rem; color:#8b949e; margin-top:40px; }

    /* ====== RESPONSIVIDADE ====== */
    @media (max-width:768px){
      header { flex-direction:column; align-items:flex-start; }
      nav ul { flex-direction:column; gap:10px; margin-top:10px; }
      iframe { height:250px; }
    }
  </style>
</head>
<body>  

  <!-- ====== HEADER ====== -->  
  <header>
    <div class="logo">
      <h1>dev_silv</h1>
    </div>
    <nav>
      <ul>
        <li><a href="#sobre">Sobre</a></li>
        <li><a href="#casos">Casos</a></li>
        <li><a href="#protecao">Proteção</a></li>
        <li><a href="#video">Vídeo</a></li>
        <li><a href="#referencias">Referências</a></li>
      </ul>
    </nav>
  </header>  

  <!-- ====== SOBRE ====== -->  
  <section id="sobre">
    <h2>O que é Segurança Digital?</h2>
    <div class="card">
      <p>
        Segurança digital é a proteção de redes, programas, sistemas, sites, aplicativos e dados contra ataques virtuais.
        Provavelmente você já viu alguma vez no noticiário um caso de vazamento de dados sensíveis, como endereços de e-mail e números de CPF, quando um site é atacado e invadido por hackers.
        Para que isso não aconteça, é preciso investir em proteção digital e educação — usuários bem informados sabem proteger melhor seus dados e acessos, fazem senhas mais fortes e evitam clicar em links suspeitos.
      </p>
      <p>
        Os tipos mais comuns de ataques digitais têm como objetivo roubar dados sensíveis, como número de cartão de crédito, senhas de banco, CPF, endereço e acesso à caixa de e-mails, com finalidades como extorsão, chantagem, falsa identidade e invasão de contas.
      </p>
    </div>
  </section>  

  <!-- ====== CASOS ====== -->  
  <section id="casos">
    <h2>Casos que ocorreram</h2>
    <div class="card">
      <ul>
        <li><strong>Carolina Dieckmann (2011):</strong> Um hacker invadiu o computador da atriz, acessando 36 fotos íntimas e exigindo R$10 mil para não divulgá-las.</li>
        <li><strong>LinkedIn (2012):</strong> Vazamento expôs dados pessoais de mais de 117 milhões de usuários, incluindo e-mails e senhas.</li>
        <li><strong>Evernote (2013):</strong> Acesso não autorizado resultou no vazamento de nomes de usuários, e-mails e senhas.</li>
        <li><strong>Yahoo (2013):</strong> Vazamento de dados de 3 bilhões de usuários, incluindo nome, telefone, data de nascimento e senha.</li>
        <li><strong>Facebook/Cambridge Analytica (2014):</strong> 50 milhões de usuários tiveram informações usadas indevidamente para testes comportamentais.</li>
        <li><strong>eBay (2014):</strong> 145 milhões de contas expostas devido a credenciais de funcionários.</li>
        <li><strong>Departamento de Imigração da Austrália (2014):</strong> Dados de líderes do G20 enviados por engano por e-mail.</li>
        <li><strong>British Airways (2015):</strong> Dados de passageiros acessados sem autorização.</li>
        <li><strong>Uber (2016):</strong> Dados de 57 milhões de usuários, incluindo 200 mil brasileiros, foram roubados.</li>
        <li><strong>MySpace (2016):</strong> Dados de 360 milhões de usuários expostos e vendidos online.</li>
      </ul>
    </div>
  </section>  

  <!-- ====== PROTEÇÃO ====== -->  
  <section id="protecao">
    <h2>Como se proteger</h2>
    <div class="card">
      <ul>
        <li>Eduque e treine sua equipe constantemente para evitar golpes e links suspeitos.</li>
        <li>Siga a LGPD e proteja os dados dos clientes.</li>
        <li>Instale antivírus em todos os dispositivos.</li>
        <li>Troque senhas regularmente e use senhas fortes.</li>
        <li>Evite redes Wi-Fi públicas e habilite autenticação em dois fatores.</li>
        <li>Faça backup periódico e salve documentos em nuvem com senha.</li>
        <li>Evite uso de pendrives e dispositivos externos com dados confidenciais.</li>
      </ul>
    </div>
  </section>  

  <!-- ====== VÍDEO ====== -->  
  <section id="video">
    <h2>Vídeo recomendado</h2>
    <div class="card">
      <iframe src="https://www.youtube.com/embed/NT6ZQPlfsYE" title="Segurança Digital no YouTube" allowfullscreen></iframe>
    </div>
  </section>  

  <!-- ====== REFERÊNCIAS ====== -->  
  <section id="referencias">
    <h2>Referências</h2>
    <div class="card">
      <ul>
        <li><a href="https://contaazul.com/blog/seguranca-digital/" target="_blank">Conta Azul - Segurança Digital</a></li>
        <li><a href="https://laramartinsadvogados.com.br/artigos/28-principais-casos-de-vazamentos-de-dados-na-historia/" target="_blank">Lara Martins Advogados - Vazamentos de Dados</a></li>
      </ul>
    </div>
  </section>  

  <!-- ====== BOTÃO VOLTAR AO TOPO ====== -->
  <button id="topBtn" title="Voltar ao topo"><i class="fas fa-arrow-up"></i></button>

  <!-- ====== FOOTER ====== -->  
  <footer>
    <p>© 2025 dev_silv - Todos os direitos reservados</p>
  </footer>  

  <script>
    // ====== ANIMAÇÃO AO ROLAR ======
    const sections = document.querySelectorAll('section');
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if(entry.isIntersecting){
          entry.target.classList.add('visible');
        }
      });
    }, { threshold: 0.1 });
    sections.forEach(section => observer.observe(section));

    // ====== BOTÃO VOLTAR AO TOPO ======
    const topBtn = document.getElementById('topBtn');
    window.onscroll = function(){
      if(document.body.scrollTop > 300 || document.documentElement.scrollTop > 300){
        topBtn.style.display = "block";
      } else {
        topBtn.style.display = "none";
      }
    };
    topBtn.onclick = function(){ window.scrollTo({top:0, behavior:'smooth'}); };
  </script>
</body>
</html>


