<div align="center">

# 🧭 Guia Prático dos Meus Projetos
### Catálogo Completo de Arquitetura, Tecnologias e Demonstrações
**Por [Gabriel Silva (ryuclover)](https://github.com/ryuclover)**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gabrielmsas/)
[![GitHub Profile](https://img.shields.io/badge/GitHub-Profile-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ryuclover)
[![Status](https://img.shields.io/badge/Status-Ativo_&_Atualizado-success?style=for-the-badge)]()

<br/>

<p align="center">
  Bem-vindo ao meu índice central de projetos! Este repositório foi criado para servir como um <b>mapa detalhado de engenharia de software</b>, documentando a arquitetura, motivação, desafios técnicos, stack utilizada e links de demonstração de cada projeto que desenvolvi.
</p>

</div>

---

## 📑 Sumário Rápido

1. [Visão Geral & Tabela Comparativa](#-visão-geral--tabela-comparativa)
2. [Aplicações Web & Plataformas Interativas (Destaques)](#-aplicações-web--plataformas-interativas)
   - [🚌 Fast-Travel](#-fast-travel)
   - [▶️ Clicktube](#️-clicktube)
   - [👾 Pixelboard](#-pixelboard)
   - [📚 Serapeu](#-serapeu)
   - [🐊 mangator](#-mangator)
3. [Sistemas, Engenharia de Software & DevOps](#-sistemas-engenharia-de-software--devops)
   - [🚀 HTTP Server DevOps (Projeto Korp)](#-http-server-devops-projeto-korp)
   - [💳 Módulo de Pagamento PIX (Mercado Pago)](#-módulo-de-pagamento-pix-mercado-pago)
   - [🌽 Cornucopia](#-cornucopia)
   - [🎭 Masquerada](#-masquerada)
4. [Interfaces & UI Experience](#-interfaces--ui-experience)
   - [🏨 HÔTE Portfolio](#-hôte-portfolio)
5. [Matriz de Habilidades & Tecnologias](#-matriz-de-habilidades--tecnologias)
6. [Sobre o Autor](#-sobre-o-autor)

---

## 📊 Visão Geral & Tabela Comparativa

| Projeto | Domínio / Categoria | Tecnologias Principais | Destaque Técnico | Deploy / Acesso |
| :--- | :--- | :--- | :--- | :---: |
| **[Fast-Travel](#-fast-travel)** | Travel & Fintech | Next.js 16 (Turbopack), TypeScript, Web Scraping | Comparador de passagens e motor de vagas gratuitas/50% da **ID Jovem**. | [![Live](https://img.shields.io/badge/Live-Vercel-000?style=flat-square&logo=vercel)](https://fast-travel-phi.vercel.app) |
| **[Clicktube](#️-clicktube)** | Video Streaming | React, Node.js, Express, CSS3 | Streaming sob demanda, pré-carregamento com buffer e dark mode premium. | [![Live](https://img.shields.io/badge/Live-Vercel-000?style=flat-square&logo=vercel)](https://clicktube-wine.vercel.app) |
| **[Pixelboard](#-pixelboard)** | Games / Real-time | Node.js, WebSockets, Docker, Canvas | Arcade de xadrez e damas multiplayer com validação de regras server-side. | [![Live](https://img.shields.io/badge/Live-Vercel-000?style=flat-square&logo=vercel)](https://pixel-board-platform.vercel.app) |
| **[Serapeu](#-serapeu)** | Knowledge Sharing | Next.js, Supabase, TypeScript, Vitest | Plataforma colaborativa de tutoriais, conformidade OWASP e Row Level Security (RLS). | [![Live](https://img.shields.io/badge/Live-Vercel-000?style=flat-square&logo=vercel)](https://serapeu.vercel.app) |
| **[mangator](#-mangator)** | Reader / Catalog | React 19, Vite, TypeScript | Leitor web moderno e de alto desempenho para mangás e webcomics. | [![Live](https://img.shields.io/badge/Live-Vercel-000?style=flat-square&logo=vercel)](https://mangator.vercel.app) |
| **[Projeto Korp](#-http-server-devops-projeto-korp)** | DevOps & Observability | Go, Docker Compose, NGINX, Prometheus, Grafana, Ansible | Pipeline completa de infraestrutura: API em Go, métricas no Prometheus e automação Ansible. | [![Repo](https://img.shields.io/badge/GitHub-Repo-181717?style=flat-square&logo=github)](https://github.com/ryuclover/http-server-projeto-korp) |
| **[Módulo Mercado Pago](#-módulo-de-pagamento-pix-mercado-pago)** | Fintech & Backend | Python, Flask, SOLID, Hexagonal Architecture | Módulo independente para cobranças PIX, arquitetura hexagonal desacoplada. | [![Repo](https://img.shields.io/badge/GitHub-Repo-181717?style=flat-square&logo=github)](https://github.com/ryuclover/Modulo-mercado-pago) |
| **[Cornucopia](#-cornucopia)** | Quant / Data Science | Python, Estatística, Agregação de Sinais | Sistema quantitativo de agregação de sinais de mercado com foco em preservação de capital. | [![Repo](https://img.shields.io/badge/GitHub-Repo-181717?style=flat-square&logo=github)](https://github.com/ryuclover/cornucopia) |
| **[Masquerada](#-masquerada)** | Desktop / P2P | Electron, React 19, TypeScript, XML | Aplicativo desktop local-first para comunicação ponto a ponto (P2P) segura. | [![Repo](https://img.shields.io/badge/GitHub-Repo-181717?style=flat-square&logo=github)](https://github.com/ryuclover/Masquerada) |
| **[HÔTE](#-hôte-portfolio)** | UI/UX & Design | HTML5, CSS3, JavaScript | Interface responsiva de plataforma de eventos e hotelaria. | [![Live](https://img.shields.io/badge/Live-Vercel-000?style=flat-square&logo=vercel)](https://hote-main.vercel.app) |

---

## 🌐 Aplicações Web & Plataformas Interativas

### 🚌 Fast-Travel
> **Comparador Inteligente de Passagens de Ônibus & Motor Oficial de ID Jovem**

- 🔗 **Repositório:** [ryuclover/Fast-Travel](https://github.com/ryuclover/Fast-Travel)
- 🌐 **Demonstração Online:** [fast-travel-phi.vercel.app](https://fast-travel-phi.vercel.app)
- 🛠️ **Stack:** Next.js 16 (Turbopack, App Router), TypeScript, TailwindCSS, APIs de Mobilidade.

#### 🎯 O Problema & A Solução
Milhares de jovens de baixa renda têm direito a passagens interestaduais gratuitas (100%) ou com 50% de desconto pelo benefício federal da ID Jovem, mas encontrar quais viagens e viações possuem assentos disponíveis é historicamente burocrático e fragmentado. O **Fast-Travel** foi concebido para unificar a busca, comparar preços convencionais e identificar automaticamente a disponibilidade de assentos reservados para a ID Jovem.

#### 💡 Destaques de Engenharia
- **Next.js 16 com Turbopack:** Construído sobre a versão mais recente do framework, com renderização otimizada no servidor (SSR/Server Actions) para respostas ágeis.
- **Motor de Busca & Normalização:** Algoritmo que consome e normaliza dados de itinerários, tratando variações de nomes de rodoviárias, datas e classes de ônibus (convencional, executivo, leito).
- **Interface Focada no Usuário:** Filtros instantâneos por faixa de preço, viação, horário de embarque e tipo de desconto.

---

### ▶️ Clicktube
> **Plataforma Moderna de Compartilhamento e Streaming de Vídeo**

- 🔗 **Repositório:** [ryuclover/Clicktube](https://github.com/ryuclover/Clicktube)
- 🌐 **Demonstração Online:** [clicktube-wine.vercel.app](https://clicktube-wine.vercel.app)
- 🛠️ **Stack:** React, Node.js, Express, JavaScript, CSS3.

#### 🎯 O Problema & A Solução
Construir uma réplica funcional e de alta fidelidade de uma plataforma de streaming complexa como o YouTube, enfrentando os desafios reais de reprodução contínua de mídia, latência de carregamento e design imersivo em modo escuro.

#### 💡 Destaques de Engenharia
- **Streaming Sob Demanda & Buffer:** Estruturação para carregamento progressivo de mídia, garantindo reprodução fluida mesmo sob conexões oscilantes.
- **Arquitetura Modular:** Separação clara entre camada de componentes de player de vídeo, sugestões laterais, catálogo principal e controle de estado.
- **Experiência Premium:** Tema escuro meticulosamente desenhado com transições suaves e layout responsivo para tablets, desktops e celulares.

---

### 👾 Pixelboard
> **Plataforma Arcade Web para Jogos de Tabuleiro em Tempo Real (Multiplayer)**

- 🔗 **Repositório:** [ryuclover/Pixelboard](https://github.com/ryuclover/Pixelboard)
- 🌐 **Demonstração Online:** [pixel-board-platform.vercel.app](https://pixel-board-platform.vercel.app)
- 🛠️ **Stack:** Node.js, WebSockets, JavaScript, HTML5 Canvas/DOM, Docker.

#### 🎯 O Problema & A Solução
Jogos multiplayer na web enfrentam problemas de descompasso de estado entre jogadores (desync) e facilidade de trapaça caso a validação ocorra exclusivamente no cliente. O **Pixelboard** resolve isso através de um motor centralizado com comunicação bidirecional de baixa latência e estética retrô pixel-art.

#### 💡 Destaques de Engenharia
- **Engines de Jogo Server-Side:** O servidor valida cada jogada de **Xadrez** e **Damas** (regras de xeque, roque, en passant, capturas obrigatórias e damas), impedindo movimentos ilegais.
- **Sincronização em Tempo Real com WebSockets:** Gerenciamento dinâmico de salas, pareamento de jogadores e transmissão de eventos instantâneos.
- **Contêiner com Docker:** Arquitetura empacotada pronta para deploy rápido em plataformas como Railway e Render.

---

### 📚 Serapeu
> **Plataforma Colaborativa de Compartilhamento de Tutoriais Passo a Passo**

- 🔗 **Repositório:** [ryuclover/Serapeu](https://github.com/ryuclover/Serapeu)
- 🌐 **Demonstração Online:** [serapeu.vercel.app](https://serapeu.vercel.app)
- 🛠️ **Stack:** Next.js (App Router), Supabase (PostgreSQL, PLpgSQL), TypeScript, Vitest.

#### 🎯 O Problema & A Solução
Oferecer um ambiente robusto e seguro para criação, catalogação e leitura de guias técnicos e tutoriais práticos, onde múltiplos autores podem contribuir com integridade de dados assegurada.

#### 💡 Destaques de Engenharia
- **Row Level Security (RLS) & Segurança OWASP:** Políticas estritas de controle de acesso no PostgreSQL via Supabase, garantindo que usuários só alterem dados sobre os quais têm permissão explícita.
- **Banco de Dados Estruturado:** Uso de funções armazenadas (PLpgSQL), triggers e modelagem relacional rigorosa para gerenciar etapas de tutoriais e tags.
- **Qualidade Assegurada com Vitest:** Conjunto de testes automatizados para validação de fluxos de dados e integridade dos componentes.

---

### 🐊 mangator
> **Plataforma Moderna e Imersiva de Leitura de Mangás**

- 🔗 **Repositório:** [ryuclover/mangator](https://github.com/ryuclover/mangator)
- 🌐 **Demonstração Online:** [mangator.vercel.app](https://mangator.vercel.app)
- 🛠️ **Stack:** React 19, Vite, TypeScript, CSS3 Moderno, Vercel Serverless.

#### 🎯 O Problema & A Solução
Criar um leitor digital de alto desempenho que garanta navegação ágil entre capítulos, pré-carregamento inteligente de imagens pesadas e uma interface minimalista sem distrações para os leitores.

#### 💡 Destaques de Engenharia
- **Adoção Antecipada do React 19:** Utilização das melhorias mais recentes de concorrência e renderização do React combinadas com o empacotamento ultrarrápido do Vite.
- **Leitor Flexível:** Suporte a diferentes modos de leitura (leitura contínua vertical ou navegação tradicional página a página) adaptando-se a telas touch e navegação por teclado.

---

## ⚙️ Sistemas, Engenharia de Software & DevOps

### 🚀 HTTP Server DevOps (Projeto Korp)
> **Infraestrutura Completa: Servidor Go, Docker, NGINX, Prometheus, Grafana e Ansible**

- 🔗 **Repositório:** [ryuclover/http-server-projeto-korp](https://github.com/ryuclover/http-server-projeto-korp)
- 🛠️ **Stack:** Go (Golang), Docker, Docker Compose, NGINX, Prometheus, Grafana, Ansible.

#### 🎯 O Problema & A Solução
Demonstrar na prática uma esteira moderna de entrega e observabilidade de infraestrutura, indo do código-fonte de uma API resiliente até o seu provisionamento automatizado e monitoramento em tempo real.

#### 💡 Destaques de Engenharia
- **Servidor Nativo em Go:** API construída sem dependências desnecessárias, utilizando a biblioteca padrão `net/http` e expondo métricas operacionais para o coletor do Prometheus.
- **Proxy Reverso com NGINX:** Roteamento e isolamento de portas para proteger o tráfego que atinge os contêineres de aplicação.
- **Observabilidade Completa:** Configuração de scraping no Prometheus e dashboards visuais no Grafana para métricas de tempo de resposta, taxa de erros (HTTP 5xx/4xx) e consumo de CPU/Memória.
- **Automação com Ansible:** Playbooks estruturados para provisionar, instalar dependências e inicializar a stack de contêineres de forma reproduzível em qualquer ambiente Linux.

---

### 💳 Módulo de Pagamento PIX (Mercado Pago)
> **Módulo Desacoplado em Python/Flask com Arquitetura Hexagonal e Princípios SOLID**

- 🔗 **Repositório:** [ryuclover/Modulo-mercado-pago](https://github.com/ryuclover/Modulo-mercado-pago)
- 🛠️ **Stack:** Python, Flask, REST API, Arquitetura Hexagonal (Ports & Adapters), SOLID.

#### 🎯 O Problema & A Solução
A maioria das integrações de gateway de pagamento é fortemente acoplada ao framework web, tornando difícil migrar de ferramenta ou testar as regras de negócio de forma isolada. Este módulo oferece uma solução 100% modular e reutilizável para pagamentos instantâneos via PIX.

#### 💡 Destaques de Engenharia
- **Arquitetura Hexagonal:** O núcleo de negócio de pagamentos é totalmente independente de framework (Flask atua apenas como um adaptador de entrada HTTP).
- **Princípios SOLID:** Interfaces bem definidas para clientes HTTP e processadores de cobrança, permitindo trocar o gateway ou criar mocks para testes sem alterar a lógica interna.
- **Fluxo Completo PIX:** Geração de QR Code estático/dinâmico, chave Copia e Cola e tratamento de webhooks de notificação de pagamento.

---

### 🌽 Cornucopia
> **Sistema Quantitativo de Inteligência de Mercado e Agregação de Sinais**

- 🔗 **Repositório:** [ryuclover/cornucopia](https://github.com/ryuclover/cornucopia)
- 🛠️ **Stack:** Python, Análise Quantitativa, Modelagem de Dados, PyProject.

#### 🎯 O Problema & A Solução
Aborda a tomada de decisão no mercado financeiro a partir de uma ótica rigorosa de dados: *"Operadores que historicamente demonstraram consistência e sobrevivência estão concordando suficientemente nesta operação?"*. Em vez de focar apenas em métricas de ganho a curto prazo, o sistema prioriza a preservação de capital e convergência estatística de sinais.

#### 💡 Destaques de Engenharia
- **Filosofia Survival-First:** Modelagem baseada em mitigação de cauda longa (risco de ruína).
- **Processamento de Sinais:** Pipelines analíticos em Python estruturados para limpeza, agregação ponderada e validação de sinais históricos.

---

### 🎭 Masquerada
> **Aplicativo Desktop Local-First para Comunicação Ponto a Ponto (P2P)**

- 🔗 **Repositório:** [ryuclover/Masquerada](https://github.com/ryuclover/Masquerada)
- 🛠️ **Stack:** Electron, React 19, Vite, TypeScript, Fast-XML-Parser.

#### 🎯 O Problema & A Solução
Com o aumento de preocupações de privacidade e vigilância de dados em serviços de mensagens centralizados, o **Masquerada** adota uma abordagem **local-first** e descentralizada, permitindo a troca de mensagens diretamente entre pares na rede.

#### 💡 Destaques de Engenharia
- **Arquitetura Local-First:** Os dados pertencem ao usuário e residem na sua própria máquina.
- **Integração Desktop Nativa:** Unificação do poder do runtime do Node.js com a interface reativa moderna construída em React 19 + TypeScript dentro do Electron.

---

## 🎨 Interfaces & UI Experience

### 🏨 HÔTE Portfolio
> **Design Front-end Responsivo para Sistema de Eventos e Hotelaria**

- 🔗 **Repositório:** [ryuclover/Hote-portfolio](https://github.com/ryuclover/Hote-portfolio)
- 🌐 **Demonstração Online:** [hote-main.vercel.app](https://hote-main.vercel.app)
- 🛠️ **Stack:** HTML5 Semântico, CSS3 Moderno, JavaScript Vanilla.

#### 🎯 Destaques
- Transposição visual de um sistema complexo (originalmente modelado em Flask e MySQL) para um showcase de design focado em ergonomia visual, hierarquia de informações e compatibilidade entre navegadores.

---

## 🧩 Matriz de Habilidades & Tecnologias

A tabela abaixo relaciona as tecnologias dominadas com os projetos em que foram aplicadas na prática:

| Tecnologia / Conceito | Projetos Onde Foi Aplicado |
| :--- | :--- |
| **TypeScript** | Fast-Travel, Serapeu, mangator, Masquerada |
| **React / Next.js** | Fast-Travel (Next 16), Serapeu (Next.js), Clicktube (React), mangator (React 19), Masquerada (React 19) |
| **Node.js & Express** | Pixelboard, Clicktube |
| **Python & Flask** | Modulo-mercado-pago, Cornucopia |
| **Go (Golang)** | http-server-projeto-korp |
| **Bancos de Dados & SQL** | Serapeu (Supabase/PostgreSQL/PLpgSQL), Modulo-mercado-pago |
| **DevOps & Infraestrutura** | http-server-projeto-korp (Docker, NGINX, Prometheus, Grafana, Ansible), Pixelboard (Docker) |
| **WebSockets (Real-time)** | Pixelboard |
| **Arquitetura Hexagonal & SOLID**| Modulo-mercado-pago |
| **Segurança & Boas Práticas** | Serapeu (OWASP Top 10, Row Level Security) |
| **Testes Automatizados (TDD)** | Serapeu (Vitest), Modulo-mercado-pago (Python unittest/pytest) |

---

## 👨‍💻 Sobre o Autor

<div align="center">

### Gabriel Silva (ryuclover)
**Desenvolvedor Full Stack Júnior na [TimeSaver](https://www.linkedin.com/in/gabrielmsas/) & Graduando em Análise de Dados na UFRJ**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Gabriel_Silva-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gabrielmsas/)
[![GitHub](https://img.shields.io/badge/GitHub-ryuclover-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ryuclover)

</div>

Experiência consolidada em desenvolvimento web full stack, integrações de APIs, automação de processos para a área da saúde (healthtech) e engenharia de software resiliente. Sempre aberto a desafios técnicos estimulantes, projetos open-source e novas oportunidades.
