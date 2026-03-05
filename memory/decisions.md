# Decisões — site-nyres

## Astro puro (sem React/Vue)
- **Data:** 2026-03-05
- **Contexto:** Landing page estática com animações CSS
- **Decisão:** Astro 5 + Tailwind v4, sem frameworks JS
- **Razão:** Performance máxima, mesmo stack do site-julia

## Paleta extraída da marca real
- **Data:** 2026-03-05
- **Contexto:** Análise de logo, Instagram (@nyresedim) e fotos profissionais
- **Decisão:** Teal-deep (#1A5C5A) como primária, sand (#D4BFA0) como secundária, brown (#4A2810) para texto
- **Razão:** Consistência com identidade visual existente — Instagram usa teal overlay, logo é sand/cream

## Cormorant Garamond + Lato
- **Data:** 2026-03-05
- **Contexto:** Logo usa script fino/elegante; Instagram usa serif editorial + sans clean
- **Decisão:** Cormorant Garamond (serif refinada) + Lato (sans limpa)
- **Razão:** Combina com o tom sofisticado e acolhedor da marca

## Landing page única com seções (não multi-page)
- **Data:** 2026-03-05
- **Contexto:** Pedro perguntou se seriam páginas separadas
- **Decisão:** Home (/) = landing page autossuficiente com todas as seções. Páginas internas futuras como bônus.
- **Razão:** 90% dos visitantes resolvem tudo na home. Páginas extras são pra SEO e aprofundamento.

## Conteúdo reaproveitado do WordPress
- **Data:** 2026-03-05
- **Contexto:** Site WordPress na HostGator visualmente quebrado, mas conteúdo intacto
- **Decisão:** Extrair tudo via WP REST API e recriar em Astro
- **Razão:** Conteúdo bem escrito (irmã do Pedro), só o visual estava quebrado

## Deploy Vercel + DNS Registro.br
- **Data:** 2026-03-05
- **Decisão:** Nameservers direto da Vercel (ns1/ns2.vercel-dns.com) no Registro.br
- **Razão:** Desvincula totalmente da HostGator, opção mais limpa
