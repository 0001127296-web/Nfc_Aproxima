# Aproxima — site completo (pronto para publicar)

Site estático (HTML/CSS/JS puro), sem build e sem instalar nada. Já está completo: as fotos das placas estão dentro do `index.html`.

## Arquivos
- `index.html` — o site inteiro
- `obrigado.html` — aberta depois de enviar o pedido
- `privacidade.html` — Política de Privacidade (modelo; peça revisão profissional)
- `404.html` — página de erro
- `og.png`, `favicon.svg`, `robots.txt`, `sitemap.xml`
- `vercel.json` (usado só na Vercel) e `_headers` (usado em Cloudflare Pages e Netlify)

## Como publicar (grátis e permitido para uso comercial)
1. Crie um repositório novo no GitHub e envie estes arquivos soltos (descompacte o zip antes).
2. **Cloudflare Pages:** Workers & Pages > Create > Pages > Connect to Git > escolha o repositório. Framework: nenhum. Build command: vazio. Output directory: deixe vazio ou `/`. Salve e faça o deploy.
3. **Netlify (alternativa):** Add new site > Import from Git, ou arraste a pasta descompactada em "Deploy manually". Build command vazio; publish directory `.`
4. Anote o endereço gerado (ex.: `nome.pages.dev` ou `nome.netlify.app`) e use sempre o endereço de produção.

## Depois de publicar
O endereço `https://aprox-nfc.vercel.app` aparece em `index.html` (og:image e dados estruturados), `robots.txt`, `sitemap.xml` e `privacidade.html`/`obrigado.html` (canonical). O canonical do `index.html` se ajusta sozinho ao endereço onde o site estiver. Para trocar os demais, use "localizar e substituir" ou peça a revisão.

## Preencher quando tiver
- `resposta:""` no bloco `CFG` do `index.html` e `RESP` em `obrigado.html` (prazo de resposta).
- `CASES=[]` no `index.html`: casos reais, só com autorização do cliente.
