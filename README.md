# diariodotreinador.com.br

Site estático do ecossistema **Diário do Treinador** — Gabriel Bussinger.
HTML puro, sem build. Cada página é um arquivo único (CSS e JS inline) e os assets ficam na raiz.

## Páginas

| Arquivo | Página |
|---|---|
| `index.html` | Lista de links — Diário do Treinador (hub do ecossistema) |
| `gabriel-bussinger.html` | Lista de links — Gabriel Bussinger |
| `mentoria.html` | Mentoria Diário do Treinador (página de vendas) |
| `bestsellers.html` | Best Sellers Aplicados ao Futebol (cursos) |

## Como o ecossistema se conecta

```
gabriel-bussinger.html --"Entrar no ecossistema"--> index.html
index.html --"Conhecer a mentoria"------------------> mentoria.html
index.html --"Ver os cursos"------------------------> bestsellers.html
index.html --"voltar"-------------------------------> gabriel-bussinger.html
mentoria.html --"voltar"----------------------------> index.html
mentoria.html --"Ver o curso Best Sellers"----------> bestsellers.html
bestsellers.html --"voltar"-------------------------> index.html
bestsellers.html --"Conheça a Mentoria"-------------> mentoria.html
```

## Publicar no GitHub Pages

1. Crie o repositório e suba estes arquivos na raiz (branch `main`).
2. Settings → Pages → Source: `Deploy from a branch` → `main` / `/ (root)`.
3. Para usar o domínio próprio, em Settings → Pages → Custom domain digite
   `www.diariodotreinador.com.br` (o GitHub cria o arquivo `CNAME` sozinho) e
   aponte o DNS: `CNAME www → <usuario>.github.io`.

## Pendências de conteúdo

- `curso-comece-pelo-porque.mp4` **não está no repositório** (arquivo original tem 497 MB).
  Reexporte em ~1080p / H.264 / ~4 Mbps (alvo 20–60 MB) e coloque na raiz, ou troque o
  `<video>` de `bestsellers.html` por um embed do YouTube/Vimeo.
  Enquanto isso o player mostra o poster `poster-comece-pelo-porque.jpg`.
- `mentoria.html`: os botões do plano anual e do plano mensal apontam para a **mesma**
  oferta da Hotmart (`I103504037F?off=nhfhufix`). Falta o link do plano mensal.
- `index.html`: o link "Suporte" usa `wa.me/5551991736138`, que é o mesmo número do
  crédito "Feito por Sttudio11WD" no rodapé. Conferir se o suporte deve ir para outro número.
- `index.html`: "Banco de Profissionais" está marcado como indisponível, sem destino.
- Revisar as traduções EN/ES das quatro páginas.
- `bestsellers.html`: preencher a duração do curso e publicar os outros seis títulos
  (hoje resumidos na frase "Os demais títulos do catálogo entram em breve").

## Créditos

Design e desenvolvimento: Sttudio11WD.
