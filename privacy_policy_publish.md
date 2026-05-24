# Publicar politica de privacidade na Cloudflare Pages

## O que publicar

Use o arquivo `docs/privacy-policy.html`.

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

1. Criar um repositorio ou pasta publica com `index.html`.
2. Usar o conteudo de `docs/privacy-policy.html` como `index.html`.
3. Publicar no Cloudflare Pages.
4. Copiar a URL final, por exemplo:
   `https://politica.truckly.pages.dev`
5. Colar essa URL na Play Console.

## Onde usar na Play Console

- `Detalhes do app -> Politica de privacidade`
- Se aplicavel, repita a mesma URL nas secoes de `Acesso ao app` e `Seguranca dos dados`, quando a Play Console pedir contexto adicional.

## Observacao importante

Se o app acessar dados pessoais ou sensiveis, o Google Play pode exigir que a politica tambem esteja acessivel dentro do app, alem da ficha da loja.
