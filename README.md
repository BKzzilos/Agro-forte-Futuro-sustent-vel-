# Agro forte, Futuro sustentável
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Farming Simulator - Agro Forte, Futuro Sustentável</title>

  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700&family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">

  <style>

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      scroll-behavior:smooth;
    }

    body{
      font-family:'Poppins', sans-serif;
      background:#111827;
      color:white;
      overflow-x:hidden;
    }

    nav{
      position:fixed;
      top:0;
      width:100%;
      padding:18px 8%;
      display:flex;
      justify-content:space-between;
      align-items:center;
      background:rgba(0,0,0,0.75);
      backdrop-filter:blur(10px);
      z-index:1000;
    }

    nav h1{
      font-family:'Orbitron', sans-serif;
      color:#84cc16;
      font-size:24px;
    }

    nav ul{
      display:flex;
      list-style:none;
      gap:25px;
    }

    nav ul li a{
      color:white;
      text-decoration:none;
      transition:0.3s;
      font-weight:500;
    }

    nav ul li a:hover{
      color:#84cc16;
    }

    header{
      height:100vh;
      background:
      linear-gradient(rgba(0,0,0,0.65), rgba(0,0,0,0.7)),
      url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1600&auto=format&fit=crop');

      background-size:cover;
      background-position:center;
      display:flex;
      justify-content:center;
      align-items:center;
      text-align:center;
      padding:20px;
    }

    .hero{
      max-width:900px;
    }

    .hero h2{
      font-size:65px;
      font-family:'Orbitron', sans-serif;
      margin-bottom:20px;
      color:#bef264;
      text-shadow:0 0 20px rgba(132,204,22,0.6);
    }

    .hero p{
      font-size:20px;
      margin-bottom:35px;
      color:#e5e7eb;
    }

    .btn{
      display:inline-block;
      padding:15px 35px;
      background:#84cc16;
      color:#111827;
      text-decoration:none;
      border-radius:50px;
      font-weight:bold;
      transition:0.3s;
      box-shadow:0 0 20px rgba(132,204,22,0.5);
    }

    .btn:hover{
      transform:translateY(-4px);
      background:#a3e635;
    }

    section{
      padding:100px 8%;
    }

    .titulo{
      text-align:center;
      margin-bottom:60px;
    }

    .titulo h2{
      font-size:45px;
      color:#bef264;
      font-family:'Orbitron', sans-serif;
      margin-bottom:15px;
    }

    .titulo p{
      max-width:700px;
      margin:auto;
      color:#d1d5db;
    }

    .cards{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
      gap:30px;
    }

    .card{
      background:#1f2937;
      padding:35px;
      border-radius:20px;
      border:1px solid rgba(132,204,22,0.3);
      transition:0.4s;
      box-shadow:0 10px 25px rgba(0,0,0,0.3);
    }

    .card:hover{
      transform:translateY(-10px);
      border-color:#84cc16;
      box-shadow:0 0 30px rgba(132,204,22,0.25);
    }

    .card h3{
      color:#bef264;
      margin-bottom:15px;
      font-size:24px;
    }

    .impactos{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
      gap:25px;
    }

    .impacto{
      background:linear-gradient(145deg,#1f2937,#111827);
      padding:40px;
      border-radius:20px;
      text-align:center;
      border:1px solid rgba(132,204,22,0.3);
    }

    .impacto h3{
      font-size:55px;
      color:#84cc16;
      margin-bottom:10px;
      font-family:'Orbitron', sans-serif;
    }

    .maquinas{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
      gap:25px;
    }

    .maquina{
      position:relative;
      overflow:hidden;
      border-radius:20px;
    }

    .maquina img{
      width:100%;
      height:320px;
      object-fit:cover;
      transition:0.5s;
    }

    .maquina:hover img{
      transform:scale(1.08);
    }

    .overlay{
      position:absolute;
      inset:0;
      background:linear-gradient(transparent, rgba(0,0,0,0.8));
      display:flex;
      align-items:flex-end;
      padding:25px;
    }

    .overlay h3{
      color:#bef264;
      font-size:28px;
    }

    .contato{
      max-width:800px;
      margin:auto;
      background:#1f2937;
      padding:40px;
      border-radius:20px;
      border:1px solid rgba(132,204,22,0.2);
    }

    form{
      display:grid;
      gap:20px;
    }

    input, textarea{
      padding:15px;
      border:none;
      border-radius:10px;
      background:#111827;
      color:white;
      font-size:16px;
    }

    textarea{
      resize:none;
      height:150px;
    }

    button{
      padding:15px;
      border:none;
      border-radius:10px;
      background:#84cc16;
      color:#111827;
      font-size:16px;
      font-weight:bold;
      cursor:pointer;
      transition:0.3s;
    }

    button:hover{
      background:#a3e635;
    }

    footer{
      background:black;
      text-align:center;
      padding:30px;
      margin-top:50px;
      color:#9ca3af;
    }

    @media(max-width:768px){

      .hero h2{
        font-size:40px;
      }

      nav{
        flex-direction:column;
        gap:10px;
      }

      nav ul{
        flex-wrap:wrap;
        justify-content:center;
      }

    }

  </style>
</head>

<body>

  <nav>
    <h1>🚜 FARMING SIMULATOR</h1>

    <ul>
      <li><a href="#sobre">Sobre</a></li>
      <li><a href="#tecnologia">Tecnologia</a></li>
      <li><a href="#impactos">Impactos</a></li>
      <li><a href="#maquinas">Máquinas</a></li>
      <li><a href="#contato">Contato</a></li>
    </ul>
  </nav>

  <header>

    <div class="hero">

      <h2>
        AGRO FORTE,<br>
        FUTURO SUSTENTÁVEL
      </h2>

      <p>
        Inspire-se no universo Farming Simulator:
        tecnologia, máquinas gigantes e sustentabilidade
        trabalhando juntas para transformar o futuro do campo.
      </p>

      <a href="#sobre" class="btn">Explorar Fazenda</a>

    </div>

  </header>

  <section id="sobre">

    <div class="titulo">

      <h2>O FUTURO DO AGRO</h2>

      <p>
        Agricultura moderna com inovação,
        eficiência e respeito ao meio ambiente.
      </p>

    </div>

    <div class="cards">

      <div class="card">

        <h3>🌱 Agricultura Sustentável</h3>

        <p>
          Técnicas modernas reduzem desperdícios
          e aumentam a preservação ambiental.
        </p>

      </div>

      <div class="card">

        <h3>🚜 Máquinas Inteligentes</h3>

        <p>
          Colheitadeiras e tratores de última geração
          aumentam produtividade no campo.
        </p>

      </div>

      <div class="card">

        <h3>☀️ Energia Renovável</h3>

        <p>
          Fazendas sustentáveis usam energia solar
          e biocombustíveis para reduzir impactos.
        </p>

      </div>

      <div class="card">

        <h3>🌎 Preservação Ambiental</h3>

        <p>
          Produção eficiente sem destruir
          florestas e recursos naturais.
        </p>

      </div>

    </div>

  </section>

  <section id="impactos">

    <div class="titulo">

      <h2>RESULTADOS SUSTENTÁVEIS</h2>

    </div>

    <div class="impactos">

      <div class="impacto">
        <h3>+60%</h3>
        <p>Economia de água</p>
      </div>

      <div class="impacto">
        <h3>+45%</h3>
        <p>Maior produtividade</p>
      </div>

      <div class="impacto">
        <h3>+80%</h3>
        <p>Eficiência agrícola</p>
      </div>

      <div class="impacto">
        <h3>100%</h3>
        <p>Compromisso ambiental</p>
      </div>

    </div>

  </section>

  <section id="maquinas">

    <div class="titulo">

      <h2>MÁQUINAS DO CAMPO</h2>

      <p>
        Inspirado no visual épico de Farming Simulator.
      </p>

    </div>

    <div class="maquinas">

      <div class="maquina">

        <img src="https://images.unsplash.com/photo-1592982537447-7440770cbfc9?q=80&w=1400&auto=format&fit=crop">

        <div class="overlay">
          <h3>Tratores Modernos</h3>
        </div>

      </div>

      <div class="maquina">

        <img src="https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1400&auto=format&fit=crop">

        <div class="overlay">
          <h3>Colheita Inteligente</h3>
        </div>

      </div>

      <div class="maquina">

        <img src="https://images.unsplash.com/photo-1500382017468-9049fed747ef?q=80&w=1400&auto=format&fit=crop">

        <div class="overlay">
          <h3>Gestão Sustentável</h3>
        </div>

      </div>

    </div>

  </section>

  <section id="contato">

    <div class="titulo">

      <h2>ENTRE NA FAZENDA</h2>

      <p>
        Participe da evolução do agro sustentável.
      </p>

    </div>

    <div class="contato">

      <form>

        <input type="text" placeholder="Seu nome" required>

        <input type="email" placeholder="Seu e-mail" required>

        <textarea placeholder="Digite sua mensagem"></textarea>

        <button type="submit">Enviar Mensagem</button>

      </form>

    </div>

  </section>

  <footer>

    <p>
      © 2026 - Farming Simulator Inspired Website | Agro Forte, Futuro Sustentável
    </p>

  </footer>

  <script>

    const form = document.querySelector("form");

    form.addEventListener("submit", function(e){

      e.preventDefault();

      alert("🚜 Mensagem enviada com sucesso!");

      form.reset();

    });

  </script>

</body>
</html>
