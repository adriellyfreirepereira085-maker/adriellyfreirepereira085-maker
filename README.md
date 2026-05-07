<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Portfólio Adrielly</title>

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family: 'Poppins', sans-serif;
    }

    body{
      background: linear-gradient(135deg, #ffb6d9, #ff69b4, #ffc0cb);
      background-size: 300% 300%;
      animation: fundoAnimado 8s ease infinite;
      color: white;
      min-height: 100vh;
      display:flex;
      justify-content:center;
      align-items:center;
      padding:40px;
    }

    @keyframes fundoAnimado {
      0%{
        background-position: 0% 50%;
      }
      50%{
        background-position: 100% 50%;
      }
      100%{
        background-position: 0% 50%;
      }
    }

    .card{
      background: rgba(255,255,255,0.12);
      backdrop-filter: blur(12px);
      border: 1px solid rgba(255,255,255,0.2);
      padding:40px;
      border-radius:25px;
      max-width:850px;
      width:100%;
      box-shadow:0 8px 30px rgba(0,0,0,0.2);

      animation: aparecer 1.5s ease;
    }

    @keyframes aparecer{
      from{
        opacity:0;
        transform:translateY(40px);
      }
      to{
        opacity:1;
        transform:translateY(0);
      }
    }

    h1{
      font-size:3rem;
      margin-bottom:10px;
      animation: brilho 2s infinite alternate;
    }

    @keyframes brilho{
      from{
        text-shadow:0 0 10px #fff;
      }
      to{
        text-shadow:0 0 25px #ffebf5;
      }
    }

    .subtitle{
      font-size:1.2rem;
      margin-bottom:25px;
      color:#ffe4f1;
    }

    .info{
      line-height:2;
      font-size:1.1rem;
    }

    .section{
      margin-top:35px;
    }

    h2{
      color:#fff;
      margin-bottom:15px;
      position:relative;
      display:inline-block;
    }

    h2::after{
      content:'';
      width:100%;
      height:3px;
      background:white;
      position:absolute;
      left:0;
      bottom:-5px;
      border-radius:10px;
      animation: linha 2s infinite alternate;
    }

    @keyframes linha{
      from{
        transform:scaleX(0.5);
      }
      to{
        transform:scaleX(1);
      }
    }

    .skills{
      display:flex;
      flex-wrap:wrap;
      gap:12px;
      margin-top:15px;
    }

    .skill{
      background: rgba(255,255,255,0.2);
      padding:10px 18px;
      border-radius:30px;
      transition:0.3s;
      cursor:pointer;
    }

    .skill:hover{
      transform:scale(1.1);
      background:white;
      color:#ff1493;
      box-shadow:0 0 15px white;
    }

    .email{
      margin-top:15px;
      font-weight:bold;
      color:#fff;
    }

    p{
      line-height:1.8;
      color:#fff5fa;
    }

    .emoji{
      animation: flutuar 2s infinite ease-in-out;
      display:inline-block;
    }

    @keyframes flutuar{
      0%{
        transform:translateY(0px);
      }
      50%{
        transform:translateY(-5px);
      }
      100%{
        transform:translateY(0px);
      }
    }

  </style>
</head>

<body>

  <div class="card">

    <h1>Olá <span class="emoji">👋</span>, eu sou Adrielly Freire</h1>

    <div class="subtitle">
      🎯 Desenvolvedora Backend em formação
    </div>

    <div class="info">
      💻 Formada em Ciência da Computação <br>
      📚 Aluna de DS no SENAC <br>
      🌱 Atualmente aprimorando minhas habilidades em Java, Spring Boot, APIs REST e Bancos de Dados <br>
      🌍 Buscando oportunidades internacionais
    </div>

    <div class="section">
      <h2>📧 Email</h2>

      <div class="email">
        adriellyfreirepereira085@gmail.com
      </div>
    </div>

    <div class="section">
      <h2>🚀 Linguagens e Ferramentas</h2>

      <div class="skills">
        <div class="skill">Java</div>
        <div class="skill">Spring Boot</div>
        <div class="skill">MySQL</div>
        <div class="skill">HTML</div>
        <div class="skill">CSS</div>
        <div class="skill">JavaScript</div>
        <div class="skill">Git</div>
        <div class="skill">GitHub</div>
      </div>
    </div>

    <div class="section">
      <h2>💖 Sobre mim</h2>

      <p>
        Graduada em Ciência da Computação com foco em desenvolvimento backend utilizando Java e Spring Boot.
      </p>

      <br>

      <p>
        Atualmente desenvolvendo projetos práticos envolvendo APIs REST, banco de dados e integração com aplicações web.
      </p>

      <br>

      <p>
        Buscando aprimorar conhecimentos em arquitetura de software, desenvolvimento de APIs e boas práticas de programação.
      </p>

      <br>

      <p>
        Tenho grande interesse em aprender continuamente, resolver problemas e desenvolver aplicações utilizadas no mundo real.
      </p>

    </div>

  </div>

</body>
</html>
