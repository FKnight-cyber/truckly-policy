# Publicar politica de privacidade na Cloudflare Pages

## O que publicar

Use o arquivo `docs/index.html`.

Antes de subir:

1. Troque `SEU_EMAIL_DE_SUPORTE_AQUI` por um email real.
2. Se algum ponto do app mudar (ex.: camera, localizacao, assinatura paga, analytics), atualize a politica.

## Como publicar rapido na Cloudflare Pages

Uma pagina estatica na Cloudflare Pages resolve bem este requisito, desde que:

- a URL seja publica
- abra sem login
- use HTTPS
- nao retorne erro 404

Fluxo simples:

1. Conectar este repositorio no Cloudflare Pages.
2. Configurar `Build command` como vazio.
3. Configurar `Build output directory` como `docs`.
4. Publicar o projeto.
5. Copiar a URL final, por exemplo:
   `https://politica.truckly.pages.dev`
6. Colar essa URL na Play Console.

## Como publicar com Wrangler

Se voce preferir manter o deploy command como `npx wrangler deploy`, este repositorio ja inclui um `wrangler.toml` apontando para `docs/`.

Configuracao:

1. Use `Deploy command` = `npx wrangler deploy`.
2. Nao precisa de build command.
3. O Wrangler vai publicar os arquivos estaticos de `docs/`.

## Onde usar na Play Console

- `Detalhes do app -> Politica de privacidade`
- Se aplicavel, repita a mesma URL nas secoes de `Acesso ao app` e `Seguranca dos dados`, quando a Play Console pedir contexto adicional.

## Observacao importante

Se o app acessar dados pessoais ou sensiveis, o Google Play pode exigir que a politica tambem esteja acessivel dentro do app, alem da ficha da loja.
