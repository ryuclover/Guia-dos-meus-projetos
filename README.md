<div align="center">

# 🧭 Guia Prático dos Meus Projetos
### Aplicações, extensões, infraestrutura e experimentos
**Por [Gabriel Silva (ryuclover)](https://github.com/ryuclover)**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gabrielmsas/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ryuclover)

Um mapa do meu portfólio, com o objetivo de cada projeto, tecnologias, decisões de engenharia e caminhos para testar ou explorar o código.

**Última revisão: 30 de outubro de 2026.** · [Repositório deste guia](https://github.com/ryuclover/Guia-dos-meus-projetos)

</div>

## 📑 Navegação

- [Visão geral](#visao-geral)
- [Extensões e ferramentas criativas](#ferramentas-criativas): Wide Studio e Photopea AI Studio
- [Aplicações web e plataformas](#aplicacoes-web): BeeHost, Fast-Travel, Clicktube, Pixelboard, Serapeu e mangator
- [Desktop, dados e infraestrutura](#sistemas): Masquerada, Projeto Korp, Módulo Mercado Pago e Cornucopia
- [Interfaces e portfólio](#interfaces): portfólio pessoal e HÔTE
- [Matriz de tecnologias](#tecnologias)
- [Sobre o autor](#autor)

<a id="visao-geral"></a>

## 📊 Visão geral

| Projeto | Categoria | Tecnologias principais | Acesso |
| :--- | :--- | :--- | :--- |
| [Wide Studio](#wide-studio) | Extensão / edição de vídeo | TypeScript, extensão de navegador, wide.video | [Download](https://github.com/ryuclover/wide-studio/releases/latest) |
| [Photopea AI Studio](#photopea-ai-studio) | Plugin / edição de imagem com IA | React, TypeScript, Vite, SDXL | [Repositório](https://github.com/ryuclover/photopea-ai-studio) |
| [BeeHost](#beehost) | Hospedagem de jogos / cloud | React, TypeScript, Node.js, Asaas, Daytona | [Repositório](https://github.com/ryuclover/BeeHost) |
| [Fast-Travel](#fast-travel) | Mobilidade / comparação de passagens | Next.js, TypeScript, APIs, web scraping | [Demo](https://fast-travel-phi.vercel.app) |
| [Clicktube](#clicktube) | Compartilhamento de vídeos | React, Express, MongoDB, Cloudinary | [Demo](https://clicktubeapp.vercel.app) |
| [Pixelboard](#pixelboard) | Jogos multiplayer | React, Express, Socket.io, Prisma, PostgreSQL | [Demo](https://pixel-board-platform.vercel.app) |
| [Serapeu](#serapeu) | Compartilhamento de conhecimento | Next.js, Supabase, PostgreSQL, Vitest | [Demo](https://serapeu.vercel.app) |
| [mangator](#mangator) | Catálogo / leitura de quadrinhos | React, TypeScript, Vite | [Demo](https://mangator.vercel.app) |
| [Masquerada](#masquerada) | Comunicação desktop P2P | Electron, React, TypeScript, WebRTC, SQLite | [Download](https://github.com/ryuclover/Masquerada/releases/latest) |
| [Projeto Korp](#projeto-korp) | DevOps / observabilidade | Go, Docker, NGINX, Prometheus, Grafana, Ansible | [Repositório](https://github.com/ryuclover/http-server-projeto-korp) |
| [Módulo Mercado Pago](#mercado-pago) | Integração de pagamentos PIX | Python, Flask, SQLAlchemy | [Repositório](https://github.com/ryuclover/Modulo-mercado-pago) |
| [Cornucopia](#cornucopia) | Análise quantitativa / dados | Python, SQLite, pytest | [Repositório](https://github.com/ryuclover/cornucopia) |
| [Portfólio pessoal](#portfolio-pessoal) | Apresentação profissional | HTML, CSS, JavaScript | [Site](https://site-six-gules-60.vercel.app) |
| [HÔTE](#hote) | Interface de eventos | HTML, CSS, JavaScript | [Demo](https://hote-main.vercel.app) |

Os links de demonstração são os publicados pelos projetos; a disponibilidade pode variar. Para instalação e requisitos completos, consulte o README de cada repositório.

<a id="ferramentas-criativas"></a>

## 🎬 Extensões e ferramentas criativas

<a id="wide-studio"></a>

### Wide Studio

Extensão independente que reorganiza o workspace do **wide.video** e adiciona ferramentas para importar mídia e trabalhar na timeline.

- **Stack:** TypeScript e integração com o editor wide.video no navegador.
- **Recursos:** navegação em pastas públicas do Google Drive, prévia e importação de arquivos, importação de vídeos por URL, seleção por retângulo, vínculo entre clipes, histórico, menus personalizáveis e tradução da interface.
- **Engenharia:** módulos separados para workspace, bridge de comunicação, Drive, extração, seleção, vínculos e internacionalização; testes automatizados e cenários reais de navegador documentados no repositório.
- **Limites:** importações por URL dependem de serviços externos; vínculos e preferências ficam no navegador. O chat de edição assistida é experimental e tem ações limitadas.

**[Código e documentação](https://github.com/ryuclover/wide-studio#readme) · [Baixar a extensão](https://github.com/ryuclover/wide-studio/releases/latest)**

**Como experimentar:** extraia o ZIP da release, ative o modo de desenvolvedor em `chrome://extensions` ou equivalente e carregue a pasta `extensao`. Abra o wide.video na versão indicada no README.

**Desenvolvimento:** na pasta `extension`, execute `npm ci` e `npm run build`; carregue `extension/dist` como extensão descompactada. Verificações: `npm run typecheck`, `npm test` e `npm run test:ui`.

<a id="photopea-ai-studio"></a>

### Photopea AI Studio

Plugin experimental para alterar áreas selecionadas de uma imagem com IA e inserir o resultado como **nova camada**, preservando a original.

- **Stack:** React, TypeScript, Vite e integração com SDXL no Hugging Face.
- **Fluxo:** captura da seleção do canvas, prompt, geração, prévia, ajustes locais de borda e inserção no Photopea.
- **Engenharia:** integração com o documento e a seleção, testes com fixtures e cenários de canvas e integração no navegador.
- **Limites:** o provedor público pode ter fila e cota de GPU; remoção de objetos e troca de cor nem sempre atendem ao pedido. Imagens e prompts são enviados ao provedor escolhido. Outros provedores exigem configuração própria e não foram todos validados.

**[Código, demonstração e instalação](https://github.com/ryuclover/photopea-ai-studio#readme)**

**Como executar:** com Node.js 22.18+ e npm, rode `npm ci` e `npm run dev`. Abra a URL do Vite, clique em **Abrir no Photopea** e acesse o painel **AI Studio**. Verificações: `npm test`, `npm run lint` e `npm run build`.

<a id="aplicacoes-web"></a>

## 🌐 Aplicações web e plataformas

<a id="beehost"></a>

### BeeHost

Plataforma de venda, provisionamento e gerenciamento de servidores **Minecraft PaperMC**, conectando uma vitrine pixel art ao fluxo de pagamento e à infraestrutura em nuvem.

- **Stack:** React, TypeScript, Tailwind CSS, Vite, Node.js, Asaas, Daytona Cloud, PaperMC e Crafty Controller.
- **Recursos:** catálogo de planos, checkout PIX com QR Code, confirmação por webhook, área do cliente com ações de energia e painel administrativo.
- **Engenharia:** separação entre vitrine, API de pagamentos e orquestração; scripts de provisionamento, tunelamento e migração; interface em português e inglês e efeitos com Web Audio API.
- **Demonstração:** o projeto documenta um modo de simulação de pagamento para explorar o fluxo local. Pagamentos e provisionamento reais dependem das credenciais e serviços configurados.

**[Código, capturas e guia completo](https://github.com/ryuclover/BeeHost#readme)**

**Como executar:** instale com `npm install`, copie `.env.example` para `.env` e siga a configuração do README. Em terminais separados, rode `npm run backend` e `npm run dev`. Verificações: `npm test` e `npm run build`.

<a id="fast-travel"></a>

### Fast-Travel

Comparador de passagens de ônibus que reúne buscas por origem, destino e intervalo de datas, com consulta de disponibilidade de benefícios **ID Jovem** e links para os provedores.

- **Stack:** Next.js, TypeScript, Tailwind CSS, APIs e web scraping.
- **Engenharia:** integração de múltiplos provedores, normalização de itinerários, comparação de tarifas e filtros por viação, horário e classe.
- **Objetivo:** reduzir a busca manual em diferentes sites e datas. A disponibilidade e a confirmação do benefício dependem dos dados retornados pelos provedores.

**[Demo](https://fast-travel-phi.vercel.app) · [Código e execução local](https://github.com/ryuclover/Fast-Travel#readme)**

<a id="clicktube"></a>

### Clicktube

Plataforma de compartilhamento e reprodução de vídeos inspirada no YouTube.

- **Stack:** React, Vite, Node.js, Express, MongoDB/Mongoose e Cloudinary.
- **Recursos:** player com atalhos de teclado, Picture-in-Picture, pré-carregamento e barra de buffer; feed com rolagem infinita, busca e navegação para visitantes.
- **Engenharia:** API separada por controllers, autenticação JWT em cookies HTTP-only, validação de consultas e upload de mídia para Cloudinary.

**[Demo indicada no README](https://clicktubeapp.vercel.app) · [Código e execução local](https://github.com/ryuclover/Clicktube#readme)**

<a id="pixelboard"></a>

### Pixelboard

Arcade de **xadrez e damas**, com partidas locais, contra o computador e multiplayer online.

- **Stack:** React, Vite, Express, Socket.io, Prisma, PostgreSQL/Neon, chess.js e Docker.
- **Recursos:** matchmaking, salas, temporizador, desistência, proposta de empate, perfis, conquistas e ranking.
- **Engenharia:** validação de movimentos no servidor, sincronização de estado via Socket.io e tratamento de reconexão durante as partidas.

**[Demo](https://pixel-board-platform.vercel.app) · [Código, configuração do banco e execução](https://github.com/ryuclover/Pixelboard#readme)**

<a id="serapeu"></a>

### Serapeu

Plataforma colaborativa para criar, organizar e compartilhar tutoriais passo a passo.

- **Stack:** Next.js, React, TypeScript, Supabase, PostgreSQL/PLpgSQL e Vitest.
- **Recursos:** tutoriais com blocos de código, autenticação, perguntas e solicitações da comunidade, votação e administração.
- **Engenharia:** Row Level Security, controle de papéis no banco, funções e triggers, proteção de fluxos de autenticação e testes automatizados.

**[Demo](https://serapeu.vercel.app) · [Código, arquitetura e execução](https://github.com/ryuclover/Serapeu#readme)**

<a id="mangator"></a>

### mangator

Aplicação de catálogo e leitura de mangás, webtoons e quadrinhos.

- **Stack:** React, TypeScript, Vite, CSS e funções serverless na Vercel.
- **Recursos:** catálogo com filtros, detalhes e capítulos, leitor vertical, atalhos de teclado e favoritos no armazenamento local.
- **Engenharia:** pré-carregamento de imagens e navegação entre capítulos, com interface adaptada a diferentes tamanhos de tela.

**[Demo](https://mangator.vercel.app) · [Código e execução local](https://github.com/ryuclover/mangator#readme)**

<a id="sistemas"></a>

## ⚙️ Desktop, dados e infraestrutura

<a id="masquerada"></a>

### Masquerada

Aplicação desktop de comunicação **P2P e local-first**, com organização em servidores e canais.

- **Stack:** Electron, React, TypeScript, Vite, WebRTC e SQLite.
- **Recursos:** mensagens, chamadas de voz, compartilhamento de tela e histórico local.
- **Engenharia:** integração do runtime desktop com a interface React, persistência na máquina do usuário e conexões entre pares via WebRTC.

**[Download para Windows](https://github.com/ryuclover/Masquerada/releases/latest) · [Código, arquitetura e execução](https://github.com/ryuclover/Masquerada#readme)**

<a id="projeto-korp"></a>

### HTTP Server DevOps — Projeto Korp

Desafio de infraestrutura que parte de uma API HTTP em Go e inclui empacotamento, proxy reverso, observabilidade e provisionamento.

- **Stack:** Go, Docker Compose, NGINX, Prometheus, Grafana e Ansible.
- **Engenharia:** servidor com `net/http`, métricas para Prometheus, dashboard provisionado no Grafana e playbooks Ansible para subir o ambiente.
- **Como executar:** siga o README da branch padrão para rodar a API com `go run main.go` ou a stack com `docker compose up -d --build`.

**[Código, arquitetura e guia de execução](https://github.com/ryuclover/http-server-projeto-korp#readme)**

<a id="mercado-pago"></a>

### Módulo de Pagamento PIX — Mercado Pago

Módulo reutilizável para integrar cobranças PIX a aplicações Flask.

- **Stack:** Python, Flask, SQLAlchemy e API Mercado Pago.
- **Recursos:** criação e consulta de pagamentos, QR Code, código Copia e Cola, sincronização de status e webhook.
- **Engenharia:** arquitetura hexagonal e princípios SOLID para separar regras de negócio, persistência e integração HTTP.
- **Como executar:** instale `requirements.txt`, configure o `.env` com suas credenciais e integre `PixPaymentModule` à aplicação Flask conforme o README. Testes: `python -m unittest tests.test_module -q`.

**[Código, endpoints e integração](https://github.com/ryuclover/Modulo-mercado-pago#readme)**

<a id="cornucopia"></a>

### Cornucopia

Sistema quantitativo de análise e agregação de sinais de traders, com foco em consistência, sobrevivência e preservação de capital.

- **Stack:** Python, SQLite, empacotamento via `pyproject.toml` e pytest.
- **Engenharia:** separação entre performance, score e peso; eventos de execução imutáveis, contabilidade FIFO, ingestão CSV/JSON, replay cronológico, avaliação e ranking históricos.
- **Modelagem:** cálculos ponto-no-tempo, preservação do histórico de coortes e análise de dependência entre traders para estudar vieses e redundância de sinais.

**[Código, etapas e guia técnico](https://github.com/ryuclover/cornucopia#readme)**

<a id="interfaces"></a>

## 🎨 Interfaces e portfólio

<a id="portfolio-pessoal"></a>

### Portfólio pessoal — ryuclover.github.io

Site de apresentação profissional com seções sobre trajetória, tecnologias, projetos e contato.

- **Stack:** HTML, CSS e JavaScript.
- **Interface:** layout em cartões, tema escuro e conteúdo em português e inglês.
- **Como explorar:** abra `index.html` no navegador ou acesse o site publicado.

**[Site](https://site-six-gules-60.vercel.app) · [Código](https://github.com/ryuclover/ryuclover.github.io)**

<a id="hote"></a>

### HÔTE Portfolio

Versão estática do front-end de um dos meus primeiros sistemas de eventos, originalmente desenvolvido em Flask e MySQL.

- **Stack desta versão:** HTML, CSS e JavaScript.
- **Interface:** páginas inicial, sobre, serviços e contato, preservando a identidade visual e a navegação do projeto original.
- **Como executar:** abra `index.html` no navegador. Este repositório apresenta o front-end estático.

**[Demo](https://hote-main.vercel.app) · [Código e detalhes](https://github.com/ryuclover/Hote-portfolio#readme)**

**Outros repositórios:** [infinity-dungeon](https://github.com/ryuclover/infinity-dungeon) ainda estava vazio nesta revisão. O repositório [ryuclover](https://github.com/ryuclover/ryuclover) contém o README do perfil, e este guia funciona como índice central.

<a id="tecnologias"></a>

## 🧩 Matriz de tecnologias

| Tecnologia / conceito | Projetos em que aparece |
| :--- | :--- |
| TypeScript | Wide Studio, Photopea AI Studio, BeeHost, Fast-Travel, Serapeu, mangator, Masquerada |
| React / Next.js | Photopea AI Studio, BeeHost, Fast-Travel, Clicktube, Pixelboard, Serapeu, mangator, Masquerada |
| Extensões e integração com editores | Wide Studio, Photopea AI Studio |
| IA generativa / SDXL | Photopea AI Studio |
| Node.js / Express | BeeHost, Clicktube, Pixelboard |
| Python | Cornucopia, Módulo Mercado Pago |
| Go | Projeto Korp |
| PostgreSQL / Supabase / Prisma | Serapeu, Pixelboard |
| MongoDB / Cloudinary | Clicktube |
| SQLite | Masquerada, Cornucopia |
| PIX e webhooks | BeeHost (Asaas), Módulo Mercado Pago |
| Tempo real / P2P | Pixelboard (Socket.io), Masquerada (WebRTC) |
| Infraestrutura e automação | BeeHost (Daytona, PaperMC, Crafty), Projeto Korp (Docker, NGINX, Ansible), Pixelboard (Docker) |
| Observabilidade | Projeto Korp (Prometheus, Grafana) |
| Arquitetura hexagonal / SOLID | Módulo Mercado Pago |
| Segurança e controle de acesso | Serapeu (RLS e políticas no banco), Clicktube (autenticação e validação), Pixelboard (validação no servidor) |
| Testes automatizados | Wide Studio, Photopea AI Studio, BeeHost, Serapeu, Cornucopia, Módulo Mercado Pago |
| HTML / CSS / JavaScript | Portfólio pessoal, HÔTE |

<a id="autor"></a>

## 👨‍💻 Sobre o autor

**Gabriel Silva (ryuclover)** — Desenvolvedor Full Stack na TimeSaver e graduando em Análise de Dados na UFRJ.

Trabalho com aplicações web, integrações de APIs, automação de processos e soluções para healthtech. Nos projetos pessoais, exploro também ferramentas criativas, comunicação P2P, análise de dados e infraestrutura.

**[LinkedIn](https://www.linkedin.com/in/gabrielmsas/) · [GitHub](https://github.com/ryuclover)**
