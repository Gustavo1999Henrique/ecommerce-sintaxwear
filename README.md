# 👟 SintaxWear - Tênis e Sneakers Online

<div align="center">
  <img src="./images/logo/logo.svg" alt="SintaxWear Logo" width="280">
  <br><br>
  <p><b>Uma landing page e-commerce moderna, elegante e responsiva para a marca de sneakers SintaxWear.</b></p>

  [![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
  [![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/CSS)
  [![Responsivo](https://img.shields.io/badge/Design-Responsivo-7c3aed?style=for-the-badge)](#-responsividade)
</div>

---

## 📖 Sobre o Projeto

O **SintaxWear** é um projeto de landing page de e-commerce focado na apresentação e venda de tênis e sneakers exclusivos. O projeto foi construído utilizando boas práticas de desenvolvimento front-end com **HTML5 semântico** e **CSS3 modular**, destacando os produtos em um layout moderno, dinâmico e focado em experiência do usuário (UX/UI).

---

## ✨ Funcionalidades e Destaques

- **Navegação Fixa e Flutuante (Header):** Menu suspenso sobreposto ao banner inicial, com ícones de navegação rápida e alternância para menu hambúrguer em telas menores.
- **Seção Hero Impactante:** Destaque para o lançamento do modelo **Krypton One** com botões interativos de chamada para ação (*Call To Action* - CTA).
- **Galeria de Categorias:** Seção de filtragem visual (Casual, Esporte, Moderno, Futurista) com máscaras de overlay escuro e transições.
- **Grid de Produtos Assimétrico (CSS Grid):** Disposição dinâmica em grade destacando modelos principais em diferentes proporções de tela.
- **Rodapé Completo (Footer):** Formulário de inscrição em newsletter, links diretos de redes sociais e mapa de navegação do site.
- **Totalmente Responsivo:** Adaptado perfeitamente para dispositivos móveis, tablets e computadores de alta resolução.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5 Semântico:** Uso correto de tags como `<header>`, `<main>`, `<section>`, `<nav>`, `<article>` e `<footer>` para melhor acessibilidade e SEO.
- **CSS3 Avançado:**
  - **Flexbox** para alinhamento de componentes e menus.
  - **CSS Grid** para construção da galeria assimétrica de produtos.
  - **Variáveis CSS (`:root`)** para centralização de fontes e temas de cores.
  - **Arquitetura Modular:** Separação de estilos por responsabilidade (Reset, Base, Variáveis e Componentes).
- **Google Fonts:** Tipografia da família [*Ubuntu*](https://fonts.google.com/specimen/Ubuntu) (pesos 300, 400, 500, 700).
- **Vetor SVG:** Ícones de interface leves e infinitamente escaláveis.

---

## 📁 Estrutura de Pastas e Arquivos

```text
ecommerce-sintaxwear/
├── index.html                  # Estrutura principal da página
├── README.md                   # Documentação detalhada do projeto
├── css/                        # Arquivos de estilização CSS
│   ├── base.css                # Estilos base globais e botões reutilizáveis
│   ├── reset.css               # Reset de margens e padding padrões do navegador
│   ├── variables.css           # Variáveis CSS e importação de fontes
│   └── components/             # Estilos modulares por componente
│       ├── footer.css          # Estilos do rodapé, newsletter e redes sociais
│       ├── header.css          # Estilos do menu superior e menu mobile
│       ├── hero.css            # Estilos da seção banner principal (Hero)
│       ├── product-category.css# Estilos dos cards de categorias
│       └── product-grid.css    # Estilos do layout em grade dos produtos
└── images/                     # Recursos visuais e mídias do site
    ├── banners/                # Imagens de fundo para a seção Hero (Desktop e Mobile)
    │   ├── hero.jpg
    │   └── hero-mobile.jpg
    ├── icons/                  # Ícones da interface em SVG (Carrinho, Usuário, Redes Sociais, etc.)
    │   ├── bag.svg
    │   ├── facebook.svg
    │   ├── hamburguer.svg
    │   ├── help.svg
    │   ├── instagram.svg
    │   ├── tiktok.svg
    │   ├── user.svg
    │   └── whatsapp.svg
    ├── logo/                   # Logotipo oficial em formato vetorial SVG
    │   └── logo.svg
    └── products/               # Imagens em alta definição dos sneakers e modelos
        ├── Image_Example.png
        ├── card_imagem.jpg
        ├── casual.jpg
        ├── esporte.jpg
        ├── futurista-grid.jpg
        ├── futurista.jpg
        ├── modelo-femino.jpg
        ├── moderno-grid.jpg
        ├── moderno.jpg
        ├── preto-branco-grid.jpg
        └── roxo-verde-grid.jpg
```

---

## 🎨 Componentes & Design System

### 1. Header (`header.css`)
- Menu suspenso com `position: fixed` e bordas arredondadas.
- Efeito hambúrguer puro com CSS (técnica `checkbox` sem dependência de JavaScript).
- Ícones vetoriais com efeito *hover* em opacidade.

### 2. Seção Hero (`hero.css`)
- Fundo em alta resolução com troca dinâmica para versão mobile (`hero-mobile.jpg`).
- Botões padronizados `.btn-outline` (borda branca com fundo transparente) e `.btn-filled` (preenchimento branco com texto roxo).

### 3. Categorias (`product-category.css`)
- Cards verticais com overlay escuro (`rgba(0, 0, 0, 0.25)`) para aumentar o contraste dos textos e botões centrais.

### 4. Grid de Produtos (`product-grid.css`)
- Layout em **CSS Grid** de 4 colunas por 3 linhas no desktop:
  ```css
  grid-template-areas:
      "highlight highlight sneaker-purple sneaker-purple"
      "highlight highlight model sneaker-color"
      "sneaker-white sneaker-white model sneaker-silver";
  ```
- Reorganização automática para 2 colunas e rolagem suave no mobile.

---

## 📱 Responsividade

O projeto foi construído no formato **Desktop-First** com suporte completo a múltiplos pontos de interrupção (*breakpoints*):

| Dispositivo | Largura Máxima | Adaptação |
| :--- | :--- | :--- |
| **Desktop / Monitores** | `> 1280px` | Exibição em container centralizado de `1360px` com menu completo |
| **Notebooks & Tablets** | `<= 1280px` | Menu simplificado com botão hambúrguer gaveta |
| **Tablets Padrão** | `<= 768px` | Reestruturação do Grid de produtos e Banner Hero mobile dedicado |
| **Smartphones** | `<= 500px` | Cards de categorias expandem para ocupação total de tela (`100%`) |

---

## 🚀 Como Executar o Projeto

Como o projeto é construído estritamente com **HTML5** e **CSS3**, não há necessidade de instalar dependências de pacotes ou compiladores complexos.

1. **Clonar ou Baixar o Repositório:**
   ```bash
   git clone https://github.com/Gustavo1999Henrique/ecommerce-sintaxwear.git
   ```

2. **Navegar até a pasta do projeto:**
   ```bash
   cd ecommerce-sintaxwear
   ```

3. **Abrir no Navegador:**
   - Basta dar um duplo clique no arquivo [`index.html`](file:///C:/Users/Administrador/Downloads/Programation/Programation/devquest/ecommerce-sintaxwear/index.html) ou abrir através de uma extensão como o **Live Server** no VS Code.

---

## 📝 Licença & Créditos

Projeto desenvolvido como parte dos estudos de desenvolvimento front-end do curso **DevQuest**.

Desenvolvido com 💜 por [Gustavo Henrique](https://github.com/Gustavo1999Henrique).
