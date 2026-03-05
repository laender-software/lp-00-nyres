# Status do Projeto — site-nyres

- **Branch:** main
- **Build:** ✅ passa (Astro static, ~1s)
- **Deploy:** ✅ Vercel — https://site-nyres.vercel.app
- **Domínio:** nyresedim.com.br (DNS apontado pra Vercel, aguardando propagação)
- **Repo:** https://github.com/pedrolaender/site-nyres (privado)
- **Última atualização:** 2026-03-05

## Features

| Feature | Status | Notas |
|---------|--------|-------|
| Scaffold Astro + Tailwind | ✅ | Astro 5.18, Tailwind v4, Google Fonts |
| Layout base + SEO | ✅ | OG tags, canonical, sitemap |
| Header responsivo | ✅ | Sticky, hamburger mobile, scroll shadow |
| Hero | ✅ | Foto profissional Tati Motta, 2 CTAs |
| Dores do público (6 cards) | ✅ | Grid responsivo, card-lift hover |
| O que é Pathwork | ✅ | Seção teal-deep, foto profissional |
| Como Funciona (5 etapas) | ✅ | Timeline com números interativos |
| Sobre a Nyres | ✅ | Foto, bio, +25 anos experiência |
| Depoimentos | ✅ | 4 depoimentos reais (M.B., T.S., M.R., L.P.) |
| FAQ | ✅ | 4 perguntas, accordion nativo |
| CTA Final | ✅ | Seção teal-deep, WhatsApp |
| WhatsApp flutuante | ✅ | Botão fixo com float animation |
| Micro-animações | ✅ | Scroll reveal, hover zoom, card lift, button glow, stagger |
| Fotos profissionais | ✅ | Ensaio Tati Motta (3 fotos usadas) + logo |
| Paleta real da marca | ✅ | Extraída do logo, Instagram e fotos |
| Domínio custom | ⏳ | DNS configurado, propagação pendente |
| JSON-LD Schema | ❌ | Therapist + LocalBusiness |
| Astro `<Image>` otimizado | ❌ | Usando `<img>` por enquanto |
| prefers-reduced-motion | ❌ | Animações não respeitam ainda |
| robots.txt | ✅ | Configurado |
| Páginas internas | ❌ | /sobre, /pathwork, /atendimento (futuro) |

## Infraestrutura

| Componente | Status | Detalhe |
|------------|--------|---------|
| Hospedagem | ✅ Vercel | Plano gratuito, conta pedrolaender |
| Repo | ✅ GitHub | pedrolaender/site-nyres (privado) |
| CI/CD | ✅ Auto | Vercel auto-deploy via GitHub push |
| Domínio | ⏳ | nyresedim.com.br → ns1/ns2.vercel-dns.com (propagando) |

## Conteúdo

- **Fonte:** Extraído do WordPress anterior (HostGator) via WP REST API
- **Fotos:** Ensaio fotográfico por Tati Motta Fotografia (2025)
- **Depoimentos:** 4 reais do site WordPress (M.B., T.S., M.R., L.P.)
- **WhatsApp:** +55 31 98585-0589

## Próximos Passos

- [ ] Confirmar propagação DNS
- [ ] Migrar `<img>` para Astro `<Image>`
- [ ] Adicionar JSON-LD Schema (Therapist + LocalBusiness)
- [ ] Implementar prefers-reduced-motion
- [ ] Feedback da Nyres sobre visual/cores
- [ ] Confirmar duração real das sessões (FAQ tá aproximado)
- [ ] Adicionar fotos adicionais quando disponíveis
- [ ] Criar páginas internas (/sobre, /pathwork, /atendimento)
