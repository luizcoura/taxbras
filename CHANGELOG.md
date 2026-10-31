# Changelog

Todas as mudanças relevantes do projeto. Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/). O site não tem versões numeradas; as entradas são por data.

## 2026-10-30

### Adicionado
- Página principal (`index.html`) explicando a reforma tributária (CBS, IBS, Imposto Seletivo): como é hoje, o que muda, calendário 2026–2033, MEI, Pix, clubes e associações, Imposto de Renda e glossário.
- Simuladores em abas: consumidor, MEI, clube e Pix.
- Página de perguntas frequentes (`perguntas.html`) com 18 perguntas em 5 grupos, cada uma com endereço próprio (`#pix-taxado`, `#mei-acaba` etc.).
- Licença MIT, com aviso de autoria no rodapé do site.
- SEO: meta tags, URL canônica, Open Graph, Twitter Card, JSON-LD, `robots.txt` e `sitemap.xml`.
- Imagem de pré-visualização `og-image.png` (1200×630).
- Favicon em SVG, PNG 48 e `apple-touch-icon.png`.
- Publicação no GitHub Pages: https://luizcoura.github.io/reset-tributario/

### Alterado
- Simuladores: a alíquota de referência foi separada em dois campos, CBS (padrão 8,8%) e IBS (padrão 17,7%), com a soma exibida. Zerar um deles testa o outro sozinho. Os resultados do consumidor e do Pix mostram quanto do imposto é CBS e quanto é IBS.
- Projeto renomeado de `taxbras` para **RESET tributário** (Reforma Explicada Sem Enrolação Tributária); repositório `reset-tributario`.
- CSS extraído do `index.html` para `style.css`, compartilhado pelas duas páginas.

### Corrigido
- Conteúdo revisado contra fontes oficiais: alíquota de referência (teto legal de 26,5%, estimativas entre 26,5% e 28%), regras do MEI, motivo do monitoramento do Pix, clubes e Imposto de Renda.
- Tabelas do MEI e do clube escondiam a coluna "Com a reforma" no celular; agora viram cartões empilhados.
- Texto cortado nas opções do seletor do simulador de clube.
