# Paula Campos – Link na Bio

Site estático (HTML + Tailwind CDN) para a consultora imobiliária **Paula Campos**.

## Estrutura

```
biopaulasite/
├─ public/                 # Pasta servida publicamente
│  ├─ index.html
│  └─ assets/
│     └─ images/
│        ├─ mansao.jfif
│        ├─ perfil.jpg
│        ├─ perfil 2.jpg
│        └─ perfil3.png
├─ .gitignore
├─ vercel.json
└─ README.md
```

## Deploy

### Vercel (recomendado)

1. Conecte o repositório no Vercel.
2. O arquivo `vercel.json` já aponta a pasta `public` como output.
3. Deploy automático a cada push na `main`.

### Hostinger / Hospedagem tradicional

1. Faça upload do conteúdo da pasta `public/` para a raiz do seu domínio (public_html).
2. Certifique-se de que o arquivo `index.html` esteja na raiz.

## Desenvolvimento local

```bash
# Servir a pasta public com um servidor estático simples
npx serve public
# ou
python -m http.server 8000 --directory public
```

Acesse `http://localhost:8000` (ou a porta indicada) para visualizar.

## Tecnologias

- HTML5 sem build
- Tailwind CSS via CDN
- Google Fonts (Cormorant Garamond & Manrope)

## Imagens

- `mansao.jfif` – hero background (480 px altura)
- `perfil3.png` – avatar (110 px círculo)
- Outras imagens mantidas para possível uso futuro.

---

*Projeto mantido com foco em performance (width/height, fetchpriority, lazy‑loading) e SEO básico.*