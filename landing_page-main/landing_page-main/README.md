# 🎬 MovieCity — Landing Page

Landing page responsiva de um serviço de streaming fictício, desenvolvida com **React + Vite**.

O projeto foi desenvolvido como um exercício prático de desenvolvimento front-end, com foco em **componentização, CSS puro e responsividade** para diferentes tamanhos de tela.

---

## 📌 Sobre o projeto

O **MovieCity** é uma página de filmes que apresenta uma interface simples e responsiva.

A página possui:

- Logo MovieCity
- Menu de navegação
- Botão de Login
- Área de apresentação dos filmes
- Botão "Mais"
- Grid com 6 cards de filmes
- Menu hambúrguer para dispositivos menores
- Layout responsivo para computadores, tablets e celulares

Os filmes apresentados são:

- Afterlife
- Transformers
- Mowgli
- Shift
- Round 6
- Harry Potter

---

## 🛠️ Tecnologias utilizadas

O projeto foi desenvolvido utilizando:

- **React 19** — criação da interface e componentes
- **Vite 7** — ambiente de desenvolvimento e build
- **JavaScript (ESM)** — linguagem utilizada no projeto
- **CSS3** — estilização e responsividade
- **ESLint** — análise e padronização do código

Não foram utilizadas bibliotecas de interface como Bootstrap, Tailwind ou styled-components. O objetivo foi praticar **CSS puro**.

---

## 📋 Pré-requisitos

Antes de executar o projeto, é necessário ter instalado:

- Node.js 20.19+ ou 22.12+
- npm
- Visual Studio Code ou outro editor de código

Para verificar se o Node.js e o npm estão instalados:

```bash
node -v
npm -v
```

---

## 🚀 Como executar o projeto

### 1. Clonar ou baixar o projeto

Baixe o projeto para o seu computador e abra a pasta no terminal.

### 2. Entrar na pasta

```bash
cd 01_landinpage
```

### 3. Instalar as dependências

```bash
npm install
```

### 4. Iniciar o servidor de desenvolvimento

```bash
npm run dev
```

Depois, abra no navegador o endereço apresentado pelo Vite, normalmente:

```text
http://localhost:5173
```

---

## 📁 Estrutura do projeto

```text
01_landinpage/
│
├── public/
│
├── src/
│   ├── assets/
│   │   ├── afterlife.jpg
│   │   ├── transformers.jpg
│   │   ├── mowgli.jpg
│   │   ├── shift.png
│   │   ├── squidgame.webp
│   │   └── harrypotter.jpg
│   │
│   ├── components/
│   │   ├── Header.jsx
│   │   ├── Main.jsx
│   │   └── Home.jsx
│   │
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
│
├── index.html
├── eslint.config.js
├── package.json
└── vite.config.js
```

---

## 🧩 Componentes

### `App.jsx`

É o componente principal da aplicação. Ele importa o CSS global e renderiza o componente `Home`.

### `Home.jsx`

Funciona como o container principal da página, reunindo:

- `Header`
- `Main`

### `Header.jsx`

Responsável pelo cabeçalho da página.

Possui:

- Logo
- Links de navegação
- Botão de Login
- Menu hambúrguer

O menu hambúrguer utiliza o estado `menuOpen` para controlar sua abertura e fechamento.

### `Main.jsx`

Responsável pelo conteúdo principal da página.

Possui:

- Título "Seus Filmes"
- Texto de apresentação
- Botão "Mais"
- Grid com os seis cards de filmes

---

## 📱 Responsividade

A página foi desenvolvida para funcionar em diferentes tamanhos de tela.

Foram utilizados os seguintes breakpoints:

| Breakpoint | Aplicação |
|---|---|
| `1100px` | Ajustes de espaçamento e tipografia |
| `900px` | Colunas empilhadas e menu hambúrguer |
| `600px` | Cards organizados em duas colunas |
| `380px` | Ajustes para celulares pequenos |

O layout utiliza **Flexbox** e **CSS Grid** para organizar os elementos.

---

## 🎨 Estilização

Toda a estilização está concentrada no arquivo:

```text
src/index.css
```

O projeto utiliza:

- Flexbox
- CSS Grid
- Media Queries
- Transições
- Efeitos de hover
- Unidades relativas
- `minmax()` para o grid dos cards

A página possui fundo escuro e cards com imagens dos filmes.

---

## 🧪 Testes

Para verificar a responsividade, recomenda-se testar a aplicação nas seguintes larguras:

```text
1440px
1024px
768px
600px
375px
```

No navegador, o modo responsivo pode ser aberto utilizando:

```text
F12
```

e depois:

```text
Ctrl + Shift + M
```

Também deve ser verificado se não existe rolagem horizontal em nenhuma das resoluções.

---

## 🔍 Lint

Para verificar possíveis problemas no código:

```bash
npm run lint
```

---

## 📦 Build

Para gerar a versão de produção:

```bash
npm run build
```

O comando cria a pasta:

```text
dist/
```

---

## 👀 Preview

Para visualizar localmente a versão de produção:

```bash
npm run preview
```

---

## 🔗 Fluxo da aplicação

A estrutura de funcionamento do projeto segue o fluxo:

```text
index.html
     ↓
main.jsx
     ↓
App.jsx
     ↓
Home.jsx
    ↙   ↘
Header  Main
          ↓
        Cards
```

O `main.jsx` inicia a aplicação React, o `App.jsx` renderiza o `Home`, e o `Home` reúne os componentes `Header` e `Main`.

---

## 🎯 Objetivo do projeto

O principal objetivo do projeto é praticar conceitos fundamentais de desenvolvimento front-end, principalmente:

- Criação de componentes React
- Organização de projetos
- Uso de JavaScript
- Estilização com CSS puro
- Flexbox
- CSS Grid
- Responsividade
- Menu interativo com React
- Boas práticas de organização de código

---

## 💡 Possíveis melhorias

Como próximos passos, o projeto pode receber novas funcionalidades, como:

- Transformar os cards em botões
- Adicionar título e nota aos filmes
- Buscar filmes através de uma API
- Renderizar os filmes dinamicamente utilizando `.map()`
- Criar um carrossel horizontal para dispositivos móveis
- Adicionar suporte a `prefers-reduced-motion`
- Utilizar CSS Modules no futuro

---

## 👨‍💻 Projeto

**MovieCity — Landing Page**

Projeto desenvolvido como exercício prático de desenvolvimento web utilizando React, Vite, JavaScript e CSS puro.
