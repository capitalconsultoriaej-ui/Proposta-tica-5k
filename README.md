# Proposta Ótica 5K — Capital Consultoria Jr.

Landing page de uma página (HTML/CSS/JS puros, sem dependências de build) para apresentar a proposta de consultoria de identidade visual à Ótica 5K.

## Estrutura

- `index.html` — página completa (HTML + CSS + JS inline, sem dependências externas além das fontes do Google Fonts via CDN).
- `vercel.json` — configuração mínima da Vercel (URLs limpas e headers de segurança/cache).

Por ser um site 100% estático, não há `package.json`, build step ou dependências para instalar — a Vercel serve o `index.html` diretamente.

## Como publicar na Vercel

### Opção A — Import direto do GitHub (recomendado)

1. Crie um repositório novo no GitHub (ex: `proposta-otica-5k`).
2. Suba os arquivos `index.html`, `vercel.json` e este `README.md` para a raiz do repositório.
3. Acesse [vercel.com](https://vercel.com) e faça login (pode usar sua conta do GitHub).
4. Clique em **Add New → Project**.
5. Selecione o repositório `proposta-otica-5k` na lista (autorize o acesso da Vercel ao GitHub se for a primeira vez).
6. Em **Framework Preset**, deixe **Other** (ou "No Framework") — a Vercel detecta automaticamente que é um site estático.
7. Não é preciso configurar Build Command nem Output Directory. Clique em **Deploy**.
8. Em ~30 segundos o site estará no ar em uma URL como `https://proposta-otica-5k.vercel.app`.

Depois do primeiro deploy, qualquer novo `git push` para a branch principal atualiza o site automaticamente.

### Opção B — Deploy via CLI (sem GitHub)

Se preferir não usar um repositório:

```bash
npm install -g vercel
cd proposta-otica-5k
vercel
```

Siga as perguntas no terminal (login, nome do projeto, diretório = `./`). Ao final, a Vercel gera o link de produção.

### Domínio personalizado (opcional)

No painel do projeto na Vercel, vá em **Settings → Domains** para apontar um domínio próprio (ex: `propostaotica5k.com` ou um subdomínio da Capital Consultoria Jr.), caso queira algo mais profissional do que o link `.vercel.app`.

## Personalização rápida

- **Cores**: variáveis CSS no topo do `<style>` (`--purple-950`, `--purple-800`, `--gold`, etc.), extraídas da identidade visual da Capital Consultoria Jr.
- **Contatos**: seção `<footer>` e botões de WhatsApp/e-mail na seção `#contato` (link `https://wa.me/55...`).
- **Textos**: todo o conteúdo (contexto, escopo, cronograma, investimento) foi extraído do PDF `Proposta_Ótica_5K.pdf`; edite diretamente no `index.html` se algum valor mudar.

Esse link pode ser enviado diretamente para a proprietária da Ótica 5K.
