# Portfólio — Vinícius Lopes

Site estático desenvolvido em HTML/CSS/JS (uma única página).

## Como visualizar localmente
```bash
# opção 1: abrir direto no navegador
# dê duplo clique em index.html

# opção 2: servir localmente (recomendado)
python -m http.server 8080
# depois acesse http://localhost:8080
```

## Publicação (duas opções simples)

### 1) GitHub Pages (grátis)
1. Crie um repositório chamado `portfolio` (ou o nome que preferir) no GitHub.
2. Faça o *push* destes arquivos (`index.html`, `robots.txt`, `sitemap.xml`, `manifest.json`, etc.).
3. No GitHub, vá em **Settings » Pages** e selecione **Source: Deploy from a branch** e **Branch: main / root**.
4. O site ficará disponível em `https://seu-usuario.github.io/<nome-do-repo>/`.
5. (Opcional) Aponte um domínio próprio criando o arquivo `CNAME` com `www.seudominio.com.br` e configurando o DNS.

### 2) Netlify / Vercel (grátis)
- Crie uma conta, conecte seu GitHub e importe o repositório.
- *Build command*: **(vazio)** (site estático puro).
- *Publish directory*: **/**.
- O deploy sai automático a cada *commit*.

## Estrutura
```
.
├─ index.html
├─ robots.txt
├─ sitemap.xml
├─ manifest.json
├─ .gitignore
├─ LICENSE
└─ CNAME            # opcional: preencha com seu domínio
```

## SEO e PWA (básico)
- `sitemap.xml` e `robots.txt` ajudam na indexação.
- `manifest.json` prepara para instalar como *app* (PWA).
- Inclua um `favicon.ico`/`favicon.png` na raiz para ícone no navegador.

## Melhorias sugeridas
- Adicionar `favicon` e imagens otimizadas (WebP/AVIF).
- Incluir metatags Open Graph/Twitter para *preview*.
- Substituir ícones do CDN por *assets* locais ou versão *pinned*.
- Adicionar formulário de contato via serviço (Formspree, Getform, etc.).
- Automatizar deploy com GitHub Actions.
