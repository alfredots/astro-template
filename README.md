# Astro Starter Template

A minimal and flexible starter template for building modern, fast, and SEO-friendly websites with [Astro](https://astro.build/).

## 🚀 Features

- **Astro** 4.x
- **TypeScript** support
- **ESLint** + **Prettier** preconfigured
- **Responsive design**
- **SEO ready**
- Easy to extend and customize

## 📂 Project Structure

```plaintext
├── public/             # Static assets (favicons, images, etc.)
├── src/
│   ├── components/     # Reusable UI components
│   ├── layouts/        # Page layouts
│   ├── pages/          # Astro pages (.astro, .md, .mdx)
│   ├── styles/         # Global styles
│   └── utils/          # Utility functions
├── astro.config.mjs    # Astro configuration
├── tsconfig.json       # TypeScript configuration
├── package.json        # Dependencies and scripts
└── README.md           # Project documentation
```

### 📂 Pastas principais e papéis

- public/
  Tudo que está aqui é servido diretamente, sem passar pelo Astro. Útil para imagens, fontes e arquivos estáticos grandes.

- src/components/
  Componentes reutilizáveis. Podem ser .astro (nativos) ou de outros frameworks como React (.jsx / .tsx).

- src/layouts/
  Layouts que servem de "molde" para páginas, com slots (<slot />) para conteúdo dinâmico.

- src/pages/
  Onde as rotas são definidas automaticamente (file-based routing).

/about.astro → /about

/blog/[slug].astro → rota dinâmica.

- src/styles/
  Onde ficam estilos globais ou CSS modules.

- src/lib/ (opcional)
  Funções utilitárias, hooks (quando usando React/Vue dentro do Astro), etc.

- src/data/ (opcional)
  Dados estáticos em JSON/YAML/Markdown que podem ser carregados em build time.

### 🏗️ Como se organiza em projetos maiores

Quando o projeto cresce, é comum ver:

```ruby
src/
  ├── components/
  │   ├── ui/            # Botões, inputs, etc.
  │   ├── sections/      # Seções completas de página (hero, footer, etc.)
  ├── content/           # Usando @astro/content para Markdown/MDX
  ├── layouts/
  ├── pages/
  ├── utils/
  └── styles/
```

E também usar integrations como:

@astro/tailwind → classes utilitárias

@astro/image → otimização de imagens

@astro/mdx → suporte a MDX

## 📦 Installation

```bash
npm install
# or
pnpm install
# or
yarn install
```

## 🛠 Development

```bash
npm run dev
```

## 📦 Build

```bash
npm run build
```

## 🔍 Preview Production Build

```bash
npm run preview
```

## 📝 License

This project is licensed under the MIT License. Feel free to use and modify it for your own projects.

---

**Author:** [Alfredo Tito](https://github.com/alfredots)
