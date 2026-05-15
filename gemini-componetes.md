# gemini-componetes.md

Esta é a fonte única de verdade dos componentes HTML e CSS da plataforma Workmind (Colaborador e Landing Page).

## 1 tokens de design

```css
:root {
  /* Cores Principais */
  --wm-color-primary: #030e4f; /* Azul Marinho Enterprise */
  --wm-color-accent: #f49f1c; /* Laranja Conversão/CTA */
  --wm-color-bg: #f8fafc; /* Fundo Ice/Clean */
  --wm-color-surface: #ffffff;
  --wm-color-border: #e2e8f0;

  /* Textos */
  --wm-color-text: #0f172a;
  --wm-color-text-muted: #64748b;

  /* Feedback e Estados */
  --wm-color-success: #10b981;
  --wm-color-warning: #f59e0b;
  --wm-color-danger: #ef4444;
  --wm-color-info: #3b82f6;

  /* Bordas */
  --wm-radius-sm: 8px;
  --wm-radius-md: 12px;
  --wm-radius-lg: 16px;
  --wm-radius-xl: 24px;
  --wm-radius-full: 9999px;

  /* Sombras */
  --wm-shadow-soft: 0 10px 25px -5px rgba(3, 14, 79, 0.05);
  --wm-shadow-floating: 0 20px 40px -10px rgba(3, 14, 79, 0.1);

  /* Espaçamentos */
  --wm-space-1: 4px;
  --wm-space-2: 8px;
  --wm-space-3: 12px;
  --wm-space-4: 16px;
  --wm-space-6: 24px;
  --wm-space-8: 32px;
  --wm-space-12: 48px;
  --wm-space-16: 64px;
  --wm-space-24: 96px;
}
```

## 2 variaveis css globais e base

```css
body {
  font-family: 'Inter', sans-serif;
  background-color: var(--wm-color-bg);
  color: var(--wm-color-text);
  margin: 0;
  padding: 0;
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3, h4, h5 { margin: 0; color: var(--wm-color-primary); font-weight: 800; }
p { margin: 0; line-height: 1.6; }
a { text-decoration: none; color: inherit; transition: color 0.2s; }
button { cursor: pointer; border: none; font-family: inherit; }
```

## 16 Landing Page Components (Adicionados)

### Layout Público
*   `wm-public-app-shell`: Wrapper global da LP.
*   `wm-landing-container`: Box max-width (1200px) centralizado.
*   `wm-landing-section`: Seção padrão (`padding: var(--wm-space-24) 0`).
*   `wm-landing-header`: Barra superior fixa, fundo blur/translúcido.

### Hero e CTA
*   `wm-hero-banner`: Seção principal, flex row/column.
*   `wm-hero-badge`: Tag `Inteligência Psicossocial Corporativa`.
*   `wm-btn-company`: Botão `Sou Empresa` (Fundo Primary).
*   `wm-btn-employee`: Botão `Sou Colaborador` (Borda Primary ou Fundo Accent).

### Seções
*   `wm-section-header`: Título centralizado e max-width.
*   `wm-feature-grid`: Grid responsivo (`grid-template-columns: repeat(auto-fit, minmax(300px, 1fr))`).
*   `wm-split-section`: 50/50 Layout (Texto esquerda, Mockup direita).

### Cards Landing Page
*   `wm-lp-card`: Base de card estático (Hover effect suave).
*   `wm-trust-badge`: Cards horizontais para Trust Bar.
*   `wm-value-prop-card`: Ícone + Título + Texto Curto.
*   `wm-testimonial-card`: Box com aspas e autor.
*   `wm-faq-item`: Acordeão para perguntas frequentes.

### Elementos Visuais
*   `wm-mockup-browser`: Container imitando janela de navegador (MacOS style) para imagens do app.
*   `wm-flow-line`: Linha pontilhada conectando os passos da jornada.

---
*(O restante dos componentes da área do colaborador permanecem inalterados como definido anteriormente)*
