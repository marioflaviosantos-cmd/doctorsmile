# IM Odontologia Especializada

Site de uma página da IM Odontologia Especializada (Garanhuns/PE): Dr. Igor Andrade (CRO-PE 9503) e Dra. Milena Cerqueira (CRO-PE 9502).

Site estático: HTML, CSS e um script curto, sem build e sem dependências.

## Estrutura

```
index.html              página completa (CSS e JS embutidos)
img/                    imagens em WebP, em dois tamanhos quando faz diferença
fonts/jost-latin.woff2  fonte Jost hospedada no próprio site
favicon.png, apple-touch-icon.png
vercel.json             cache longo para img/ e fonts/, cabeçalhos de segurança
robots.txt
```

## Publicar

1. Crie um repositório no GitHub e envie esta pasta inteira:
   ```
   git init
   git add .
   git commit -m "Site IM Odontologia"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/im-odontologia.git
   git push -u origin main
   ```
2. Na Vercel: **Add New → Project → Import** o repositório.
   Framework Preset: **Other**. Sem build command, output directory em branco.
3. Depois de ligar o domínio, troque em `index.html` o `og:image` por uma URL completa
   (ex.: `https://www.seudominio.com.br/img/og-im.jpg`) para a prévia do WhatsApp/Instagram aparecer.

## Editar

Tudo fica em `index.html`. O formulário de agendamento abre o WhatsApp `(87) 98139-3968`
com nome, celular e interesse já preenchidos.
