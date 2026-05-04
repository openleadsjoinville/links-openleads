# Links Open Leads

Página estilo Linktree da Open Leads — single-page HTML estático, pronto pra deploy no Vercel.

## Stack
- HTML + CSS puro (sem build, sem dependências)
- Geist via Google Fonts
- Identidade visual alinhada ao site openleads.com.br (laranja `#FF5D0D`, dark, italic uppercase)

## Deploy no Vercel

### Opção 1 — via Dashboard (mais simples)
1. Acesse https://vercel.com/new
2. Faça upload da pasta ou conecte um repositório com estes arquivos
3. Framework Preset: **Other** (estático)
4. Build Command: *(deixar vazio)*
5. Output Directory: *(deixar vazio — usa a raiz)*
6. Deploy

### Opção 2 — via CLI
```bash
npm i -g vercel
cd "Links Open Leads"
vercel
# para produção:
vercel --prod
```

### Domínio personalizado
Após o deploy, em **Settings → Domains** adicione:
- `links.openleads.com.br`

E no DNS do domínio crie um CNAME apontando pra `cname.vercel-dns.com`.

## Estrutura

```
Links Open Leads/
├── index.html      # página única
├── vercel.json     # headers de segurança e cache
└── README.md
```

## Edição

Todos os links, ícones e textos estão dentro do `index.html` — basta editar.
Cores do tema ficam nas CSS variables no topo do `<style>` (`--primary`, `--bg`, etc.).
