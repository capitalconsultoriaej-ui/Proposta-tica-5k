# Proposta Ótica 5K — Capital Consultoria Jr.

Landing page de uma página (HTML/CSS/JS puros, sem dependências de build) para apresentar a proposta de consultoria de identidade visual à Ótica 5K.

## Como publicar no GitHub Pages

1. Crie um repositório novo (ex: `proposta-otica-5k`).
2. Suba o arquivo `index.html` (e este `README.md`, se quiser) para a raiz do repositório.
3. No repositório, vá em **Settings → Pages**.
4. Em "Build and deployment", selecione **Deploy from a branch**, branch `main`, pasta `/root`.
5. Salve — em alguns minutos o link ficará disponível em `https://<seu-usuario>.github.io/<nome-do-repo>/`.

Esse link pode ser enviado diretamente para a proprietária da Ótica 5K.

## Estrutura

- `index.html` — página completa (HTML + CSS + JS inline, sem dependências externas além das fontes do Google Fonts via CDN).

## Personalização rápida

- Cores: variáveis CSS no topo do `<style>` (`--purple-950`, `--purple-800`, `--gold`, etc.), extraídas da identidade visual da Capital Consultoria Jr.
- Contatos: seção `<footer>` e botão de WhatsApp na seção `#contato` (link `https://wa.me/55...`).
- Textos: todo o conteúdo (contexto, escopo, cronograma, investimento) foi extraído do PDF `Proposta_Ótica_5K.pdf`; edite diretamente no HTML se algum valor mudar.
