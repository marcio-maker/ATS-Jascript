ATS Landing Page
Visão Geral
Este projeto é uma Landing Page para um sistema de gerenciamento de candidatos (ATS - Applicant Tracking System). Ele inclui três páginas web:

Home (index.html): Página principal com seção hero, benefícios do ATS em carrossel, depoimentos em carrossel, formulário de contato e links para redes sociais.
Sobre (index_about.html): Página com informações sobre a empresa.
Dashboard (index_dashboard.html): Interface interativa para gerenciar candidatos, com filtros, exportação/importação de dados em JSON e integração com React e Tailwind CSS.

A Landing Page é responsiva para mobile e web, usa emojis como ícones para evitar dependência de URLs externas, possui carrosséis automáticos para benefícios e depoimentos, e inclui efeitos de hover em cards e botões. O design utiliza uma paleta de cores consistente (#1e40af, #e0f2fe, #333).
Funcionalidades

Home (index.html):
Seção hero com botão CTA ("Acesse o Dashboard") que leva ao index_dashboard.html.
Carrossel de benefícios (3 cards) com ícones (💼, 🔍, 📥), automático (5s) e com botões manuais.
Carrossel de depoimentos (3 cards) com ícones (👤), textos e autores, também automático.
Formulário de contato (estático, sem backend) e links de redes sociais (📘, 🐦, 💼, 📷).
Botão "Experimente o ATS Agora" com espaçamento aumentado (2rem mobile, 3rem web).
Efeitos de hover (escala e sombra) em cards, botões e links.
Responsividade: 1 card por vez no mobile, até 3 na web.


Sobre (index_about.html):
Descrição da empresa com botão CTA para o dashboard.
Estilo consistente com a página inicial (HTML/CSS puro).


Dashboard (index_dashboard.html):
Interface para gerenciar candidatos com filtros por status e posição.
Funcionalidades de adicionar, editar, excluir, exportar e importar candidatos (JSON).
Usa React, Tailwind CSS e Lucide Icons para uma UI moderna.


Navegação:
Header com links para Home, Sobre e Dashboard em todas as páginas.



Tecnologias

HTML5 e CSS3: Estrutura e estilo das páginas index.html e index_about.html.
JavaScript: Carrosséis automáticos, efeitos de hover e interatividade em index.html.
React e Tailwind CSS: Usados no index_dashboard.html para o dashboard interativo.
Emojis: Ícones para benefícios, depoimentos e redes sociais, garantindo funcionamento offline.

Instalação

Clone o Repositório (se aplicável):git clone <URL_DO_REPOSITORIO>


Estrutura de Arquivos:/projeto
├── index.html          # Página inicial
├── index_about.html    # Página Sobre
├── index_dashboard.html # Dashboard
└── README.md           # Este arquivo


Teste Localmente:
Abra os arquivos diretamente no navegador ou use um servidor local:python -m http.server 8000

Acesse http://localhost:8000 no navegador.
Nota: O index_dashboard.html requer internet para carregar CDNs (React, Tailwind, Lucide).


Deploy:
Hospede os arquivos em plataformas como Vercel, Netlify ou GitHub Pages.
Certifique-se de que os caminhos dos links (index.html, index_about.html, index_dashboard.html) estão corretos.



Uso

Navegação:
Use o header para alternar entre Home, Sobre e Dashboard.
Clique nos botões CTA ("Acesse o Dashboard" ou "Experimente o ATS Agora") para acessar o dashboard.


Carrosséis:
Os carrosséis de benefícios e depoimentos avançam automaticamente a cada 5 segundos.
Use os botões "←" e "→" para navegação manual.


Formulário de Contato:
O formulário é estático. Para funcionalidade, conecte a um serviço como Formspree:<form action="https://formspree.io/f/seu-id" method="POST">




Redes Sociais:
Atualize os links na seção .social-links com os URLs reais da sua empresa.



Personalização

Botão "Experimente o ATS Agora":
Ajuste o espaçamento no CSS (.benefits .cta-button):.benefits .cta-button {
  margin: 4rem 0; /* Aumentar ainda mais */
}


Modifique padding ou font-size para maior destaque.


Depoimentos e Benefícios:
Edite os textos em index.html para refletir conteúdos reais:<p>"Seu depoimento aqui."</p>
<span class="author">Nome, Cargo</span>




Ícones:
Substitua emojis por ícones SVG locais ou uma biblioteca como FontAwesome:<img src="caminho/para/icone.svg" alt="Ícone">




Carrosséis:
Altere o intervalo automático (5s) no JavaScript:setInterval(() => autoCarousel(carouselId), 3000); // 3 segundos


Para pausar no hover, adicione clearInterval no mouseenter.


Formulário:
Integre com Formspree ou um backend para processar envios.


Estilo:
Ajuste cores, fontes ou tamanhos no CSS (ex.: #1e40af para outra cor primária).



Notas

Offline: Os emojis garantem que a página funcione sem internet. Se usar ícones SVG, hospede-os localmente.
Dashboard: O index_dashboard.html depende de CDNs (React, Tailwind, Lucide). Para uso offline, baixe os recursos.
Harmonização: Para uniformizar o visual, considere reescrever index.html e index_about.html com Tailwind/React ou simplificar o dashboard para HTML/CSS puro.
Carrossel: Para recursos avançados (ex.: pausa no hover, autoplay mais configurável), considere uma biblioteca como Swiper.

Contato
Para suporte ou sugestões, envie uma mensagem via formulário na página inicial ou entre em contato pelas redes sociais (links a serem atualizados).


https://github.com/marcio-maker/ATS-Jascript/blob/main/QRCode_F%C3%A1cil.png?raw=true

© 2025 Minha Empresa. Todos os direitos reservados.
