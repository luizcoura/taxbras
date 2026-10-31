# Changelog

Todas as mudanças relevantes do projeto. Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/). O site não tem versões numeradas; as entradas são por data.

## 2026-10-30

### Corrigido (revisão técnica)
- Simuladores: CBS e IBS exibidos agora somam exatamente o imposto total (o centavo que sobra vai para o IBS); no Simples, o total da opção 2 também fecha com as parcelas.
- Simuladores: campos numéricos respeitam o `max` do HTML mesmo quando o valor é digitado (percentual de vendas para empresas e alíquotas) e limitam valores absurdos, que antes viravam infinito ou NaN.
- Modo escuro: texto em destaque do bloco de exemplo e etiqueta "estamos aqui" com contraste adequado (antes cerca de 1,2:1 e 3,1:1).
- Estilos inline movidos para `style.css`, como manda o `AGENTS.md`.
- Recibo (calendário): 2027 e 2033 não dizem mais que "acabam" todos os tributos antigos; citam a exceção do IPI na Zona Franca e a permanência do Imposto Seletivo.
- Simulador do MEI: a mensagem de excesso de faturamento agora diz que o MEI deixa de ser MEI em janeiro do ano seguinte.
- `AGENTS.md`: rótulos do DAS do MEI corrigidos (R$ 86,05 é serviços; R$ 87,05 é comércio e serviços).

### Adicionado
- Aba "Simples Nacional" nos simuladores: compara deixar CBS e IBS dentro da guia (crédito do cliente limitado ao que foi pago no DAS) com recolhê-los por fora (Simples híbrido, crédito cheio). Fontes: Fenacon e Contábeis.
- Página principal (`index.html`) explicando a reforma tributária (CBS, IBS, Imposto Seletivo): como é hoje, o que muda, calendário 2026–2033, MEI, Pix, clubes e associações, Imposto de Renda e glossário.
- Simuladores em abas: consumidor, MEI, clube e Pix (a aba do Simples Nacional veio depois).
- Página de perguntas frequentes (`perguntas.html`) com 18 perguntas em 5 grupos, cada uma com endereço próprio (`#pix-taxado`, `#mei-acaba` etc.).
- Licença MIT, com aviso de autoria no rodapé do site.
- Tag de verificação do Google Search Console no `<head>` do `index.html`. Não remover, ou o Google perde a verificação do site.
- SEO: meta tags, URL canônica, Open Graph, Twitter Card, JSON-LD, `robots.txt` e `sitemap.xml`.
- Imagem de pré-visualização `og-image.png` (1200×630).
- Favicon em SVG, PNG 48 e `apple-touch-icon.png`.
- Publicação no GitHub Pages: https://luizcoura.github.io/reset-tributario/

### Alterado
- Simulador do MEI: o custo se saísse da guia fixa e o crédito do cliente empresa agora aparecem divididos entre CBS e IBS, seguindo os dois campos de alíquota. Zerar a CBS mostra só o IBS.
- Simulador do consumidor: a linha "Alíquota efetiva" virou "Alíquota sobre o preço sem imposto", ganhou a linha "Imposto como parte do que você paga" e uma explicação da conta com a fórmula `preço × alíquota ÷ (1 + alíquota)`, para não parecer que 30% de R$ 100 deveria dar R$ 30.
- Alíquotas atualizadas com a proposta do TCU de 28/10/2026: CBS de 11,3% para 2027 (depende do Senado, prazo de 15/12) e IBS projetado em 18,7%, soma próxima de 30%. Padrões dos simuladores mudaram de 8,8% / 17,7% para 11,3% / 18,7%. Textos da página principal e da pergunta "Tudo vai ficar mais caro?" reescritos; fontes adicionadas.
- Simuladores: a alíquota de referência foi separada em dois campos, CBS e IBS (padrões iniciais 8,8% e 17,7%, trocados depois pela proposta do TCU), com a soma exibida. Zerar um deles testa o outro sozinho. Os resultados do consumidor e do Pix mostram quanto do imposto é CBS e quanto é IBS.
- Projeto renomeado de `taxbras` para **RESET tributário** (Reforma Explicada Sem Enrolação Tributária); repositório `reset-tributario`.
- CSS extraído do `index.html` para `style.css`, compartilhado pelas duas páginas.

### Corrigido
- Conteúdo revisado contra fontes oficiais: alíquota de referência (teto legal de 26,5%, estimativas entre 26,5% e 28%), regras do MEI, motivo do monitoramento do Pix, clubes e Imposto de Renda.
- Tabelas do MEI e do clube escondiam a coluna "Com a reforma" no celular; agora viram cartões empilhados.
- Texto cortado nas opções do seletor do simulador de clube.
