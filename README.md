# Dr. Darian Boccacio · Landing page

Landing page do Dr. Darian Boccacio, ortopedista com atuação em cirurgia do joelho e medicina do esporte (Jaraguá do Sul e São Bento do Sul, SC).

## Stack

- React 18 + Tailwind CSS (via CDN, sem etapa de build)
- GSAP + ScrollTrigger e Lenis para as animações e a rolagem suave
- Página única: `index.html`

## Estrutura

```
index.html          página completa (componentes React dentro do <script type="text/babel">)
assets/logo-*.png   logo (monograma e completo, fundo transparente)
assets/photos/      fotos do Dr. Darian
assets/videos/      vídeo do consultório e capa
```

## Rodar localmente

Abra com qualquer servidor estático na pasta do projeto, por exemplo:

```bash
npx serve .
```

Os vídeos e as máscaras do logo precisam ser servidos por http (não abra por `file://`).

## Antes de publicar em produção

- Gerar um build com Vite + Tailwind compilado (o Tailwind via CDN e o Babel no navegador não são indicados para produção).
- Trocar `og:image` por uma imagem hospedada no domínio final.
