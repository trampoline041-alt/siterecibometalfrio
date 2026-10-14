# Gerador de Recibo — Metalfrio Solutions

Gerador de recibo em HTML puro (sem dependências) para a Metalfrio Solutions S.A.
Preencha nome do cliente, telefone, endereço e produtos direto no navegador, e gere o PDF com o botão "Imprimir / Salvar PDF".

## Estrutura

```
.
├── index.html      # aplicação completa (HTML + CSS + JS em um único arquivo)
├── vercel.json      # configuração de deploy da Vercel
└── README.md
```

## Subir no GitHub

1. Crie um repositório novo no GitHub (ex.: `metalfrio-recibo`), sem README/gitignore automáticos.
2. No terminal, dentro desta pasta:

```bash
git init
git add .
git commit -m "Gerador de recibo Metalfrio"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/metalfrio-recibo.git
git push -u origin main
```

## Publicar na Vercel

**Opção A — pelo site:**
1. Acesse [vercel.com](https://vercel.com) e faça login (pode usar sua conta do GitHub).
2. Clique em **Add New → Project**.
3. Selecione o repositório `metalfrio-recibo` que você acabou de subir no GitHub.
4. Em "Framework Preset", escolha **Other** (é um site estático, não precisa de build).
5. Clique em **Deploy**. Em menos de um minuto o link estará no ar.

**Opção B — pela CLI:**
```bash
npm i -g vercel
vercel login
vercel --prod
```
(Rode o comando dentro desta pasta. A CLI detecta automaticamente que é um site estático.)

## Atualizações futuras

Qualquer alteração no `index.html`, basta commitar e dar `git push` — a Vercel já está conectada ao repositório e faz o redeploy automático a cada push na branch `main`.
