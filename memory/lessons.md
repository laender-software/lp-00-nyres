# Lições — site-nyres

## WP REST API funciona mesmo com tema quebrado
- **Data:** 2026-03-05
- **Descoberta:** Site WordPress visualmente destruído, mas API REST retorna todo o conteúdo estruturado
- **Aplicação:** Sempre tentar WP REST API antes de scraping manual

## Fotos profissionais no WordPress são acessíveis via /wp-json/wp/v2/media
- **Data:** 2026-03-05
- **Descoberta:** Endpoint retorna todas as imagens com URLs diretas, títulos e metadados
- **Aplicação:** Boa forma de extrair assets de sites WordPress antes de migrar

## Instagram API (RapidAPI) retorna dados em formato diferente do esperado
- **Data:** 2026-03-05
- **Descoberta:** instagram120 retorna `result.edges[].node` (não `items[]`). Precisa navegar a estrutura.
- **Aplicação:** Sempre testar o formato de resposta antes de parsear

## Vercel bloqueia deploys de commits sem Git user associado à conta
- **Data:** 2026-03-05
- **Descoberta:** Commits feitos pelo servidor (root) são bloqueados no plano Hobby
- **Solução:** Configurar `git config user.email` com o email do dono da conta Vercel
- **Aplicação:** Sempre configurar Git user correto no servidor antes de fazer push

## Registro.br mostra "Pesquisa recusada" mas salva mesmo assim
- **Data:** 2026-03-05
- **Descoberta:** Ao trocar nameservers, Registro.br testa se respondem. Vercel pode demorar. O aviso é informativo, não bloqueante.
- **Aplicação:** Ignorar o aviso e salvar — DNS propaga normalmente depois
