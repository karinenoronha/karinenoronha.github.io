# Portfólio — Karine Noronha

Site estático (HTML/CSS/JS puro, sem build) pronto para publicar no GitHub Pages.

## Estrutura

```
.
├── index.html
├── assets/
│   ├── style.css
│   ├── script.js
│   └── curriculo-karine-noronha.pdf   ← você precisa adicionar este arquivo
└── README.md
```

## ⚠️ Pendência: currículo em PDF

O botão **"Currículo (PDF)"** no topo do site aponta para:

```
assets/curriculo-karine-noronha.pdf
```

Esse arquivo ainda não existe — adicione seu currículo em PDF nessa pasta com
esse nome exato (ou troque o `href` no `index.html` por um link do Google
Drive, por exemplo, se preferir não versionar o PDF no repositório).

## Como publicar no GitHub Pages

Você tem duas opções de nome de repositório:

### Opção A — site pessoal (`usuario.github.io`)
1. Crie um repositório chamado exatamente `karinenoronha.github.io`.
2. Suba estes arquivos na raiz do repositório (branch `main`).
3. O site fica disponível automaticamente em:
   `https://karinenoronha.github.io`

### Opção B — repositório com nome próprio (igual ao site de referência)
1. Crie um repositório, por exemplo `Home` ou `portfolio`.
2. Suba estes arquivos na raiz.
3. Vá em **Settings → Pages** → em "Branch", selecione `main` e pasta `/ (root)` → **Save**.
4. O site fica disponível em:
   `https://karinenoronha.github.io/NOME-DO-REPOSITORIO/`

## Passo a passo via terminal (exemplo)

```bash
git init
git add .
git commit -m "Portfólio inicial"
git branch -M main
git remote add origin https://github.com/karinenoronha/karinenoronha.github.io.git
git push -u origin main
```

Depois, em **Settings → Pages** do repositório, confirme que a origem está
configurada como a branch `main`.

## Personalização rápida

- **Cores / fontes**: tudo centralizado nas variáveis `:root` no topo de `assets/style.css`.
- **Textos**: editar diretamente em `index.html`.
- **Novo projeto**: duplicar um bloco `<a class="project-row">...</a>` dentro da seção `#projetos` e trocar link, título, descrição e tags.
- **Foto/avatar**: o layout atual não usa foto (foco em tipografia e dados); se quiser adicionar, me avise que ajusto o hero.
