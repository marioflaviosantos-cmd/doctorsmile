# Inove Odontologia e Estética

Site de uma página da clínica Inove (Garanhuns/PE): implantes e prótese protocolo com o Dr. Eterno Freitas Jr., CRO-PE 9753.

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
   git commit -m "Site Inove"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/inove-site.git
   git push -u origin main
   ```
2. Na Vercel: **Add New → Project → Import** o repositório.
   Framework Preset: **Other**. Sem build command, output directory em branco.
3. Depois de ligar o domínio, troque em `index.html` o `og:image` por uma URL completa
   (ex.: `https://www.seudominio.com.br/img/og-inove.jpg`) para a prévia do WhatsApp/Instagram aparecer.

## Editar

Tudo fica em `index.html`. O formulário de agendamento abre o WhatsApp `(87) 98139-3968`
com nome, celular e interesse já preenchidos. Os comparadores de antes e depois usam casos clínicos
publicados no site da clínica; mantenha a autorização dos pacientes (Resolução CFO 196/2019).
