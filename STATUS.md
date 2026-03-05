# Status do Projeto — site-nyres

- **Branch:** main
- **Build:** ✅ passa (Astro static, ~1s)
- **Deploy:** ✅ Vercel — https://site-nyres.vercel.app
- **Domínio:** nyresedim.com.br ✅ LIVE — DNS via Registro.br (registro A → 76.76.21.21)
- **Repo:** https://github.com/pedrolaender/site-nyres (privado)
- **Última atualização:** 2026-03-05

## Features

| Feature | Status | Notas |
|---------|--------|-------|
| Scaffold Astro + Tailwind | ✅ | Astro 5.18, Tailwind v4, Google Fonts |
| Layout base + SEO | ✅ | OG tags, canonical, sitemap |
| Header responsivo | ✅ | Sticky, hamburger mobile, fundo teal-deep |
| Hero | ✅ | Foto profissional Tati Motta, 2 CTAs |
| Dores do público (6 cards) | ✅ | Grid responsivo, card-lift hover |
| O que é Pathwork | ❌ | Removido — conteúdo vai para FAQ expandido |
| Como Funciona (5 etapas) | ✅ | Timeline com números interativos |
| Sobre a Nyres | ✅ | Foto, bio, +25 anos experiência |
| Depoimentos | ✅ | 4 depoimentos reais (M.B., T.S., M.R., L.P.) |
| FAQ | ✅ | 4 perguntas, accordion nativo |
| CTA Final | ✅ | Seção teal-deep, WhatsApp |
| WhatsApp flutuante | ✅ | Botão fixo com float animation |
| Micro-animações | ✅ | Scroll reveal, hover zoom, card lift, button glow, stagger |
| Fotos profissionais | ✅ | Ensaio Tati Motta (3 fotos usadas) + logo |
| Paleta real da marca | ✅ | Extraída do logo, Instagram e fotos |
| Domínio custom | ✅ | nyresedim.com.br LIVE |
| JSON-LD Schema | ✅ | Person (Therapist) + LocalBusiness |
| Twitter Cards | ✅ | summary_large_image |
| Astro `<Image>` otimizado | ✅ | 4 componentes migrados, 13 variantes WebP |
| prefers-reduced-motion | ✅ | CSS + JS respeitam preferência |
| Focus styles (a11y) | ✅ | ring-2 em todos os interativos |
| Aria attributes | ✅ | hamburger, mobile nav, links |
| robots.txt | ✅ | Configurado |
| Páginas internas | ❌ | /sobre, /pathwork, /atendimento (futuro) |

## Infraestrutura

| Componente | Status | Detalhe |
|------------|--------|---------|
| Hospedagem | ✅ Vercel | Plano gratuito, conta pedrolaender |
| Repo | ✅ GitHub | pedrolaender/site-nyres (privado) |
| CI/CD | ✅ Auto | Vercel auto-deploy via GitHub push |
| Domínio | ✅ | nyresedim.com.br live — DNS Registro.br + registro A |

## Conteúdo

- **Fonte:** Extraído do WordPress anterior (HostGator) via WP REST API
- **Fotos:** Ensaio fotográfico por Tati Motta Fotografia (2025)
- **Depoimentos:** 4 reais do site WordPress (M.B., T.S., M.R., L.P.)
- **WhatsApp:** +55 31 98585-0589

## Próximos Passos

- [x] DNS nyresedim.com.br propagado e LIVE (2026-03-05)
- [x] Migrar `<img>` para Astro `<Image>` (2026-03-05)
- [x] JSON-LD Schema + Twitter Cards (2026-03-05)
- [x] prefers-reduced-motion + focus styles + aria (2026-03-05)
- [x] Header teal-deep, labels de seção em destaque (2026-03-05)
- [x] Seção "O Método" removida (2026-03-05)
- [x] Labels de seção: teal-deep + 18px (2026-03-05)
- [x] Remove link underlines globalmente (2026-03-05)
- [x] Remove imagens não usadas — design-1/2.png (2026-03-05)
- [x] Questionário para Nyres criado — docs/questionario-nyres.md (2026-03-05)
- [x] SSL/HTTPS confirmado — Vercel gerencia automaticamente (2026-03-05)
- [ ] Logo: PNG com fundo transparente (aguardando Nyres)
- [ ] FAQ expandido — aguardando respostas do questionário da Nyres
- [ ] Conteúdo: duração das sessões, horários, valores (aguardando Nyres)
- [ ] Páginas internas (/sobre, /pathwork, /atendimento) — futuro
