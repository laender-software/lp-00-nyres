# site-nyres — Nyres Edim | Terapeuta Pathwork®

Site profissional para Nyres Edim, terapeuta Pathwork® com mais de 25 anos de experiência em BH.

🌐 **Live:** [nyresedim.com.br](https://nyresedim.com.br) | [site-nyres.vercel.app](https://site-nyres.vercel.app)

## Stack

- [Astro 5](https://astro.build) (static)
- [Tailwind CSS v4](https://tailwindcss.com)
- Deploy: [Vercel](https://vercel.com)

## Desenvolvimento

```bash
npm install
npm run dev        # http://localhost:4321
npm run build      # gera dist/
npm run preview    # preview do build
```

## Estrutura

```
site-nyres/
├── public/
│   ├── images/          # Fotos profissionais + logo
│   ├── favicon.svg
│   └── robots.txt
├── src/
│   ├── components/      # Seções da landing page
│   │   ├── Header.astro
│   │   ├── Hero.astro
│   │   ├── Dores.astro
│   │   ├── Pathwork.astro
│   │   ├── ComoFunciona.astro
│   │   ├── Depoimentos.astro
│   │   ├── Sobre.astro
│   │   ├── FAQ.astro
│   │   ├── CTAFinal.astro
│   │   ├── Footer.astro
│   │   └── WhatsAppButton.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css   # @theme tokens + animações
├── memory/              # Contexto para AI agents
├── docs/                # Planos e session logs
├── CLAUDE.md            # Regras pro Claude Code
├── STATUS.md            # Estado do projeto
└── BACKLOG.md           # Tarefas pendentes
```

## Paleta

| Token | Hex | Uso |
|-------|-----|-----|
| teal-deep | #1A5C5A | Primária (botões, seções escuras) |
| teal | #5E8E91 | Acentos, links |
| sand | #D4BFA0 | Logo, CTAs em fundo escuro |
| brown | #4A2810 | Texto principal |
| cream | #F5F0EB | Fundo principal |
| warm | #EDE6DD | Fundo alternado |
