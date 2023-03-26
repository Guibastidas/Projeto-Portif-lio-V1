# Projeto-Portif-lio-V1


<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="css/style.css">
    <style>
        /* GLOBAL */

@import url("https://fonts.googleapis.com/css2?family=Rubik:wght@300&display=swap");

body {
  font-family: "Rubik", Arial, sans-serif;
  margin: 0px;
  color: #141414;
}

h1,
h2,
h3,
p {
  margin: 0px;
  padding: 0px;
  list-style: none;
}

ul {
  margin: 0px;
  padding: 0px;
  list-style: none;
}

img {
  max-width: 100%;
  display: block;
}

.subtitulo {
  font-size: 5rem;
  line-height: 1;
  text-transform: uppercase;
}

@media (max-width: 800px) {
  .subtitulo {
    font-size: 3rem;
    text-transform: capitalize;
    max-width: initial !important;
  }
}

/* HEADER */

.header {
  max-width: 1200px;
  padding: 40px 20px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.header-menu {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  justify-content: center;
}

.header-menu a {
  font-size: 1.125rem;
  line-height: 1.3;
  padding: 10px 20px;
  text-decoration: none;
  color: #141414;
  display: block;
}

@media (max-width: 800px) {
  .header {
    flex-direction: column;
    gap: 40px;
    padding: 20px;
  }

  .header a {
    background: #f5f5f5;
    border-radius: 4px;
  }
}

/* INTRODUÇÃO */

.introducao {
  max-width: 1200px;
  padding: 40px 20px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 2fr;
  gap: 100px;
  align-items: center;
}

.introducao h1 {
  font-size: 4.5rem;
  line-height: 1.125;
  margin-bottom: 30px;
  position: relative;
}

.introducao h1::before {
  content: "";
  display: block;
  width: 130px;
  height: 100px;
  background: url("/img/Detalhe.svg") no-repeat center;
  position: absolute;
  top: -20px;
  left: -50px;
  z-index: -1;
}

.introducao p {
  font-size: 1.5rem;
  color: #525252;
}

@media (max-width: 1000px) {
  .introducao h1 {
    font-size: 3rem;
  }
}

@media (max-width: 800px) {
  .introducao {
    grid-template-columns: 1fr 1fr;
    gap: 40px;
    font-size: 2rem;
  }
  
  .introducao h1::before {
    width: 30px;
    height: 10px;
    left: 0px;
  }
}

@media (max-width: 400px) {
  .introducao {
    grid-template-columns: 1fr;
  }

  .introducao img {
    display: none;
  }
}

/* EXPERIENCIA */

.projetos {
  max-width: 1200px;
  padding: 40px 20px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 2fr;
  gap: 100px;
}

.projetos .subtitulo {
  color: #e0e0e0;
}

.projetos-texto {
  font-size: 1.5rem;
  line-height: 1.33;
  max-width: 40ch;
  margin-bottom: 60px;
  color: #525252;
}

.projetos-texto strong {
  color: #141414;
}

.empresa {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 10px 20px;
  padding: 20px;
  background: #f5f5f5;
  margin-bottom: 20px;
  border-radius: 4px;
  position: relative;
}

.empresa::before {
  content: "";
  display: block;
  width: 4px;
  height: 20px;
  background: linear-gradient(#99f9f9, #0085ff);
  position: absolute;
  top: 20px;
  left: -4px;
}

.empresa-ano {
  position: absolute;
  top: 22px;
  left: -100px;
  text-align: right;
  width: 80px;
  color: #525252;
  font-size: 0.875rem;
}

.empresa-titulo {
  font-size: 1.12rem;
  line-height: 1.1;
  font-weight: bold;
}

.empresa-texto {
  font-size: 0.875rem;
  line-height: 1.4;
  color: #525252;
}

.empresa-habilidade {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  align-content: start;
}

.empresa-habilidade li {
  font-size: 0.875rem;
  line-height: 1.4;
  border-radius: 4px;
  background: #fff;
  padding: 5px 10px;
}

@media (max-width: 800px) {
  .projetos {
    grid-template-columns: 1fr;
    gap: 40px;
  }

  .projetos .subtitulo {
    color: #141414;
  }

  .projetos-texto {
    font-size: 1.25rem;
  }

  .empresa-ano {
    position: initial;
    order: 1;
    width: initial;
    text-align: left;
  }

  .empresa-ano {
    content: "Ano";
  }
}

@media (max-width: 400px) {
  .empresa {
    grid-template-columns: 1fr;
  }
}

/* FORMACAO */

.formacao {
  background: #141414;
  color: white;
}

.formacao-container {
  max-width: 1200px;
  padding: 120px 20px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 2fr;
  gap: 100px;
  position: relative;
}

.formacao-container::after {
  content: "";
  display: block;
  width: 130px;
  height: 100px;
  background: url(../img/Detalhe.svg) no-repeat center;
  position: absolute;
  bottom: -50px;
  left: 20px;
}

.formacao .subtitulo {
  color: #000000;
  max-width: 5ch;
}

.formacao-texto {
  font-size: 1.5rem;
  line-height: 1.33;
  max-width: 40ch;
  margin-bottom: 60px;
  color: #a3a3a3;
}

.formacao-texto strong {
  color: #fff;
}

.faculdade-lista {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin-bottom: 60px;
}

.faculdade {
  flex: 1;
  background: #000;
  padding: 20px;
  border-radius: 4px;
  display: flex;
  flex-direction: column;
}

.faculdade-tipo {
  font-size: .875rem;
  text-transform: uppercase;
  color: #a3a3a3;
  margin-bottom: 10px;
}

.faculdade-curso {
  flex: 1;
  font-size: 1.125rem;
  line-height: 1.4;
  margin-bottom: 40px;
  position: relative;
}

.faculdade-curso::before {
  content: "";
  display: block;
  width: 4px;
  height: 20px;
  background: linear-gradient(#99f9f9, #0085ff);
  position: absolute;
  left: -24px;
}

.faculdade-instituicao {
  font-size: 1.125rem;
  color: #a3a3a3;
}

.cursos {
  margin-bottom: 60px;
}

.formacao-extra h3 {
  font-size: .875rem;
  line-height: 1.4;
  color: #8f8f8f;
  text-transform: uppercase;
  margin-bottom: 30px;
  position: relative;
}

.formacao-extra h3::before {
  display: block;
  content: "";
  width: 24px;
  height: 24px;
  position: absolute;
  left: -36px;
  top: -4px;
}

.cursos h3::before {
  background: url(/img/cursos.svg) no-repeat center center;
}

.idiomas h3::before {
  background: url(/img/idioma.svg) no-repeat center center;
}

.formacao-extra li {
  font-size: 1.125rem;
  line-height: 1.1;
  margin-bottom: 20px;
}

.formacao-extra span {
  color: #8f8f8f;
}

.cursos li {
  display: flex;
  justify-content: space-between;
}

@media (max-width: 800px) {
  .formacao-container {
    grid-template-columns: 1fr;
    padding: 60px 20px;
    gap: 40px;
  }

  .formacao .subtitulo {
    color: #fff;
  }

  .formacao-texto {
    font-size: 1.25rem;
  }

  .formacao-extra h3::before {
    position: initial;
    margin-bottom: 10px;
  }
}

/* FOOTER */

.footer {
  background: #000;
}

.footer-container {
  max-width: 1200px;
  padding: 120px 20px 60px 20px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 2fr;
  gap: 100px;
  align-items: center;
}

.footer-texto {
  font-size: 1.5rem;
  line-height: 1.33;
  color: #cccccc;
}

.footer-contato li {
  font-weight: bold;
  font-size: 2.25rem;
  line-height: 1.1;
  color: #ffffff;
  margin-bottom: 30px;
}

.footer-contato li a {
  color: #ffffff;
}

.footer-copy {
  grid-column: 1 / -1;
  font-size: 1.125rem;
  color: #8f8f8f;
}

@media (max-width: 800px) {
  .footer-container {
    grid-template-columns: 1fr;
    gap: 40px;
  }

  .footer-contato li {
    font-size: 1.5rem;
  }
}















    </style>
    <title>Guilherme Bastidas</title>
</head>

<body>
    <header class="header">

        <a href="index.html"><img src="img/Guilherme Bastidas.svg" alt=""></a>

        <nav>
            <ul class="header-menu">
                <li><a href="#projetos">Projetos</a></li>
                <li><a href="#formacao">Formação</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
    </header>

    <main class="introducao">

        <img src="img/Perfil.png" alt="eu mesmo">

        <div>
            <h1>Desenvolvedor<br>Front-End &<br> UI Design</h1>
            <p>Localizado em Itu/Sp</p>
        </div>
    </main>
    
    <section class="projetos" id="projetos" aria-label="Projetos">
        <h2 class="subtitulo">Projetos</h2>
        <div>
            <p class="projetos-texto">Desenvolvo pequenos projetos como o Bikcraft utilizando apenas <strong>HTML</strong>, <strong>CSS</strong> e <strong>JavaScript</strong>. Atualmente me foi dada a oportunidade de <strong>recriar o site da empresa</strong> a qual orgulhosamente faço parte.</p>

            <div class="empresa">
                <span class="empresa-ano">2020 - atual</span>
                <h3 class="empresa-titulo">Caldlaser</h3>
                <span class="empresa-titulo">Helpdesk</span>
                <p class="empresa-texto">Trabalho como Helpdesk na empresa Caldlaser, trabalho cuidando da parte de infra da empresa, que diz respeito a situações que envolvem hardware. Minhas funções vão desde a preventiva dos computadores, resolver problemas com impressoras, e-mails, instalar programas e softwares.</p>
                <ul class="empresa-habilidade">
                    <li>Infraestrutura</li>
                    <li>Apontamento de Horas</li>
                    <li>Instalação de Porgramas</li>
                    <li>Preventiva das Máquinas</li>
                </ul>
            </div>

            <div class="empresa">
                <span class="empresa-ano">2022</span>
                <h3 class="empresa-titulo">Serviço Social</h3>
                <span class="empresa-titulo">Programador WEB</span>
                <p class="empresa-texto">No projeto do site SERVIÇO SOCIAL, eu e mais alguns amigos de faculdade desenvolvemos um projeto de um site, que faria um senso na cidade de Salto/Sp, para coletar dados através de um formulário e atraves da coleta desses dados gerou gráficos.</p>
                <ul class="empresa-habilidade">
                    <li>HTML</li>
                    <li>CSS</li>
                    <li>JavaScript</li>
                    <li>PHP</li>
                </ul>
            </div>

            <div class="empresa">
                <span class="empresa-ano">2023</span>
                <h3 class="empresa-titulo">Bikcraft</h3>
                <span class="empresa-titulo">Programador WEB</span>
                <p class="empresa-texto">Bikcraft foi um site criado atraves do curso de HTML e CSS da Origamid, no qual criamos um site para vendas de Bicicletas.</p>
                <ul class="empresa-habilidade">
                    <li>HTML</li>
                    <li>CSS</li>
                    <li>JavaScript</li>
                </ul>
            </div>

        </div>
    </section>

    <section class="formacao" id="formacao" aria-label="Formação">
        <div class="formacao-container">
            <h2 class="subtitulo">Formação</h2>

            <div>
                <p class="formacao-texto">
                    Minha mais recente experiência foi o <strong>curso</strong> que fiz na origamid de <strong>HTML e CSS</strong>. Além disso me mantenho sempre atualizado com cursos online envolvendo minha área.
                </p>

                <ul class="faculdade-lista">
                    <li class="faculdade">
                        <span class="faculdade-tipo">Tecnólogo</span>
                        <h3 class="faculdade-curso">Recursos Humanos</h3>
                        <span class="faculdade-instituicao">CEUNSP</span>
                    </li>
                    <li class="faculdade">
                        <span class="faculdade-tipo">Graduação</span>
                        <h3 class="faculdade-curso">Ánalise e Desenvolvimento de Sistemas</h3>
                        <span class="faculdade-instituicao">CEUNSP</span>
                    </li>
                </ul>

                <div class="formacao-extra">
                    <div class="cursos">
                        <h3>Cursos Intensivos</h3>
                        <ul>
                            <li>UX Design & UI Design <span>56h</span></li>
                            <li>Front End para Iniciantes <span>72h</span></li>
                        </ul>
                    </div>

                    <div class="idiomas">
                        <h3>Idiomas</h3>
                        <ul>
                            <li>Inglês <span>/ Fluente</span></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <footer class="footer" id="contato">
        <div class="footer-container">
            <p class="footer-texto">
                Estou disponível para novos projetos no momento. Entre em contato comigo e marcamos uma conversa.
            </p>
            <ul class="footer-contato">
                <li>bastidas.guilherme@gmail.com</li>
                <li>+55 11 97694-9046</li>
                <li><a href="/">@guibaastiidas</a></li>
            </ul>
            <p class="footer-copy">Guilherme. &copy; Alguns direitos reservados.</p>
        </div>
    </footer>

</body>

</html>
