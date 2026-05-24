# 🛒 Despensa Inteligente

Lista de compras com alertas inteligentes de estoque baseados no consumo semanal.

## Deploy no Vercel

### Opção 1 — Vercel CLI (mais rápido)

```bash
npm i -g vercel
vercel
```

### Opção 2 — GitHub + Vercel (recomendado)

1. Crie um repositório no GitHub e suba os arquivos
2. Acesse [vercel.com](https://vercel.com) → **Add New Project**
3. Importe o repositório
4. Clique em **Deploy** (sem nenhuma configuração extra)

## Estrutura de arquivos

```
despensa-vercel/
├── index.html      ← App principal (todo o código)
├── manifest.json   ← Configuração PWA
├── sw.js           ← Service Worker (offline)
├── vercel.json     ← Configuração Vercel
└── README.md
```

## Funcionalidades

- 🔴 Alerta crítico: menos de 3 dias de estoque
- 🟡 Alerta de atenção: menos de 7 dias
- 🟢 Estoque OK
- Aprende o consumo automaticamente ao marcar compras
- Funciona offline (PWA)
- Dados salvos no localStorage do navegador
