# Ana Ribeiro · Personal Trainer

Landing page e site da personal trainer Ana Ribeiro.

## Estrutura

```
AnaRibeiro/
├── index.html          # Landing estática (GitHub Pages / Vercel)
├── client/             # App React + Vite (fonte)
│   ├── index.html
│   ├── public/
│   └── src/
├── server/             # Servidor Express (produção)
├── shared/             # Código compartilhado
└── .github/workflows/  # Deploy no GitHub Pages
```

## Pré-requisitos

- Node.js 20+
- [pnpm](https://pnpm.io/) 10+

## Desenvolvimento

```bash
pnpm install
pnpm dev
```

O Vite sobe o app em `client/` (porta 3000 por padrão).

## Build e produção

```bash
pnpm build
pnpm start
```

- `pnpm build` gera os estáticos em `dist/public` e o bundle do servidor em `dist/`
- `pnpm start` sobe o Express servindo esses arquivos

## Deploy

- **GitHub Pages**: workflow em `.github/workflows/static.yml` publica a landing (`index.html` na raiz)
- **Vercel**: aponte o projeto para este repositório; a landing na raiz já funciona como site estático

## Licença

MIT
