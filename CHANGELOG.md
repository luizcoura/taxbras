# Changelog

Todas as mudanças relevantes do projeto. Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/). O site tem versão, mostrada no rodapé das duas páginas. Regra: a primeira parte muda numa reestruturação grande; a segunda, em recurso novo ou revisão de conteúdo; a terceira, em correção pontual. A 1.0.0 reúne tudo o que foi feito antes de a numeração existir.

## 1.7.0 · 2026-10-31 · quarta revisão independente

### Corrigido
- Simples: a mensagem agora compara o crédito dos dois lados. Com CBS 0,1% e IBS zero, ela diz que a opção 2 dá crédito menor (R$ 15,98 contra R$ 384,00), em vez de "crédito maior".
- Aviso dos meses de atividade: valores fora de 1 a 12 (0,6 e 12,4 inclusive) dizem "fora do limite"; só fração dentro do intervalo diz "meses inteiros".
- CBS: a expansão passou a ser "Contribuição *Social* sobre Bens e Serviços", como na LC 214 (abbr e glossário).
- "Crédito cheio" e "guia maior" saíram dos textos do MEI e da FAQ: o contador compara custos e créditos. "O preço não muda" virou "o preço depende da loja e dos impostos do produto".
- "Ficar no Simples: até 15/10" virou "pedir entrada ou retorno ao Simples", para quem já está no Simples não achar que precisa renovar.
- Mensagens do MEI e do Simples para quem vende pouco para empresas não recomendam mais "ficar na guia fixa" só pelo corte de 30%.
- Categorias dos simuladores dizem "se estiver na lista da lei" (alimento), "serviços previstos em lei" (educação) e "profissões previstas em lei"; a nota avisa que o desconto vale só para o que a lei prevê.
- FAQ: "para as empresas comuns" na frase do calendário de 2026.
- Fontes do rodapé: a notícia da Fenacon sobre o DAS (que usava R$ 1.627 antes do decreto) saiu, e entrou a notícia da Receita de 02/01/2026 (salário mínimo de R$ 1.621, Decreto 12.797/2025, que sustenta o DAS de R$ 82,05, R$ 86,05 e R$ 87,05). Mattos Filho com as datas visíveis (01/12/2025 e 17/01/2025), lista reordenada, e avisos nas fontes Contábeis (prazos superados) e Simtax (chama o 26,5% de teto).

### Alterado
- Siglas explicadas na primeira aparição: MEI no lead, IPI na nota do gráfico, CGSN, e na FAQ MEI, CBS, IBS, INSS, DAS-MEI, PLP, LC e CNPJ.
- Legibilidade: nota dos simuladores em três notas curtas; abertura do Simples em duas opções; mensalidade do clube em quatro condições com a base legal em nota pequena; mensagens de excesso do MEI mais curtas; FAQ do limite e da guia do MEI em listas.

## 1.6.0 · 2026-10-30 · terceira revisão independente

### Corrigido
- MEI que abriu no ano: a mensagem de excesso de faturamento agora mostra o valor do excesso e só o cenário calculado; acima de 20%, a saída vale desde a abertura do CNPJ (se abriu neste ano) ou desde janeiro. Mesma correção na pergunta da FAQ.
- "Na média, a taxa fica perto de 30%" virou "para uma compra sem desconto, o cenário é perto de 30%, ainda sem definição final": é um cenário, não uma média dos consumidores.
- Nota dos simuladores: não diz mais que os resultados são "como seria em 2033"; diz que são um cenário hipotético e que o quadro do MEI usa os valores de 2026.
- Simples com CBS e IBS zerados: os resultados da comparação aparecem como "indisponível", e a mensagem pede "pelo menos uma taxa maior que zero".
- Crédito: "crédito cheio" virou "pode dar crédito maior à empresa cliente que tenha direito a aproveitá-lo"; o verbete diz "quando a compra dá direito a crédito".
- Glossário: "não cumulatividade" e "por fora/por dentro" reescritos com exemplo; saiu "mais de 170 países", sem fonte.
- Split payment: o texto não diz mais que o vendedor "não precisa mais pagar a guia"; a empresa ainda apura seus tributos.
- Cashback: Cadastro Único não é mais apresentado como condição suficiente; "nada muda no bolso" da Maria virou "a guia de Maria não muda".
- Gráfico do calendário: aviso de que ele mostra o IPI zerado e não inclui o Imposto Seletivo nem o IPI residual.
- Aviso de mês fracionado diz que os meses são inteiros (antes dizia "fora do limite").
- Rodapé: a ordem das fontes é pela data de publicação visível; a Fazenda (CGSN 194) mostra a atualização de 26/10/2026 e o IBET cita os metadados.

### Alterado
- Siglas explicadas na primeira aparição em cada página (PIS, Cofins, ICMS, ISS, IPI, INSS, DAS, DAS-MEI, CSLL; na FAQ também CBS, IBS, Anvisa e PLP), com `abbr`.
- Legibilidade: parágrafo da alíquota em duas estimativas em lista; mensalidade do clube em três condições; FAQ de preços sem repetir o bloco técnico; Imposto de Renda em lista de três itens; rótulos do MEI e do Simples mais curtos ("Quanto da sua guia corresponde a CBS e IBS?").

## 1.5.0 · 2026-10-30 · linguagem para leigo

### Alterado
- Revisão de linguagem clara feita por um agente independente (nota 5/10 para leigo) e aplicada: a conclusão vem antes da lei, da data e da fonte; frases mais curtas; menos números por parágrafo.
- Parágrafo "Vai ficar mais caro?" refeito: resposta primeiro (taxa perto de 30% sobre o preço sem imposto, cerca de 23% do que se paga), depois de onde vem o número. O prazo de 15/12 do Senado agora diz "segundo a imprensa".
- Aba Simples: abertura explica as duas opções com palavras simples; prazos separados em um bloco "Até quando dá para escolher"; rótulos dos campos viraram perguntas com exemplo.
- Simulador do consumidor: o resultado abre com o imposto dentro do preço, e a conta com a fórmula fica num bloco "Ver a conta".
- Rótulos e mensagens do simulador do MEI mais curtos; mensagem de passar do limite explica "desenquadrar".
- Um nome por conceito: "regime regular" no lugar de "regime normal", "empresa cliente" no lugar de "PJ", "taxa" ao lado de "alíquota".
- Mensalidade do clube e imunidade explicadas sem artigo de lei no meio (a base legal fica no fim).
- Respostas da FAQ sobre alíquota, limite do MEI, clubes, nota fiscal e Imposto de Renda reescritas na mesma linha.
- Siglas CBS, IBS e TCU explicadas na primeira aparição (`abbr`) e aviso para o glossário no resumo.

### Corrigido
- IPI: o texto dizia "exceto para a Zona Franca", o que sugeria cobrança só lá. Agora diz que o IPI continua em alguns produtos que concorrem com os da Zona Franca de Manaus (fontes secundárias; a regulamentação não abriu).
- Pix: os limites de R$ 5 mil e R$ 15 mil agora dizem "quando passa de" e linkam a nota da Fazenda (publicada em 07/01/2025, atualizada em 27/10/2026). Saiu a frase sobre lavagem de dinheiro, que a nota não traz.
- Entrada do `CHANGELOG` da 1.2.0 sobre o art. 47, § 9º corrigida: ele trata do crédito de quem compra de empresa do Simples Nacional.

### Adicionado
- Glossário de 8 para 20 verbetes: CBS e IBS, Imposto Seletivo, PIS/Cofins/ICMS/ISS/IPI, crédito, regime regular, imposto "por fora", desenquadramento, imunidade/isenção/alíquota zero, contrapartida, CadÚnico, janela de opção e siglas de órgãos.
- Regra "Escrita para leigo" no `AGENTS.md`.

## 1.4.0 · 2026-10-30 · fontes datadas, simuladores e correções da segunda revisão

### Adicionado
- Fontes do rodapé com a data de publicação (ou de atualização) que consta em cada página, separadas em oficiais e imprensa/entidades, da mais recente para a mais antiga. Páginas sem data dizem isso; as que não abriram dizem "data não verificada".

### Removido
- Simulador do clube: aplicava alíquota cheia a bar, aluguel, eventos e aulas e rateava o crédito sem fundamento legal (a segunda revisão independente apontou o problema). A seção "E os clubes e associações?" continua explicando o assunto em texto.

### Alterado (simuladores)
- MEI: novo campo "Meses de atividade neste ano" (1 a 12); o limite passa a ser proporcional (R$ 6.750 por mês) e o faturamento anual é a média mensal vezes os meses. O rótulo do "custo extra" agora diz exatamente o que o número é: CBS e IBS líquidos estimados, sem contar o DAS que deixaria de pagar nem outros tributos.
- Pergunta sobre o limite do MEI informa o limite proporcional no ano de abertura (R$ 6.750 por mês de atividade).
- MEI e Simples: o saldo credor (compras maiores que vendas) aparece na mensagem, em vez de sumir.
- Simples: com CBS e IBS de referência zerados, a mensagem avisa que a comparação não faz sentido (antes falava em "crédito cheio" de R$ 0,00 contra R$ 384,00).
- Campos numéricos: um aviso junto do campo diz qual valor foi realmente usado quando o digitado está vazio, negativo ou acima do limite (por exemplo, "Valor fora do limite permitido. O cálculo usou 100%").

### Corrigido
- Aba Pix estourava a largura em telas de 390px (427px, e 513px com valores enormes); o rodapé também. Agora a página e as quatro abas ficam em 390px.
- Prazos do Simples híbrido: cancelamento da opção de 03/11 a 20/12/2026 e opção até 15/10 (Simples) e 30/10 (regime regular), conforme a Resolução CGSN nº 194 (Fazenda, 29/09/2026). A 1.2.0 trouxe 30/11, de uma página de abril desatualizada.
- Imunidade: "sindicatos" virou "entidades sindicais dos trabalhadores" (LC 214, art. 9º, III).
- Resumo e calendário (2033) não dizem mais que só restam CBS e IBS: citam o Imposto Seletivo e a exceção do IPI.
- Calendário de 2026: o campo novo da nota é obrigatório para o regime normal; o Simples tem calendário próprio.
- Crédito do cliente do MEI no simulador: "pouco ou nenhum" (antes "bem menor").
- Transporte público urbano: citada também a hipótese de autorização, além de permissão e concessão.
- Alíquotas dos simuladores descritas como cenário hipotético de regime completo, não "como será em 2033".

## 1.3.0 · 2026-10-30

### Adicionado
- Versão do site no rodapé do `index.html` e do `perguntas.html`, com link para este histórico de mudanças.

## 1.2.0 · 2026-10-30 · conteúdo tributário

### Corrigido (revisão independente, com fontes oficiais)
- MEI: o PLP 186/2026 foi sancionado em 21/10/2026 (R$ 110 mil em 2027 e R$ 140 mil em 2028); o texto dizia que nenhum projeto estava aprovado. Removida a menção ao PLP 108/2021, sem fonte. Fonte: Ministério do Empreendedorismo e Portal do Empreendedor.
- MEI: o crédito do cliente não cita mais o art. 47, § 9º da LC 214 como regra do MEI (esse parágrafo trata do crédito de quem compra de empresa do Simples Nacional, como confirmam fontes secundárias; esta entrada dizia, por engano, que tratava de combustíveis). Agora segue a Receita: o MEI não sofre incidência de IBS e CBS sobre as vendas, então o cliente tende a ter pouco ou nenhum crédito.
- Simples híbrido: prazos trocados por fontes oficiais. ATENÇÃO: o cancelamento até 30/11/2026 estava errado e foi corrigido na 1.4.0.
- 26,5% deixou de ser tratado como teto: é referência da LC 214 (art. 475); se a estimativa passar disso, o governo deve enviar ao Congresso projeto para reduzir a carga. Texto do site e do `AGENTS.md` ajustados.
- Associações: Imposto de Renda e CSLL "em regra" não incidem se cumprirem os requisitos da isenção; rendimentos financeiros costumam ser tributados.
- Transporte público urbano (ônibus e metrô, com permissão ou concessão) agora é isento no simulador do consumidor, conforme art. 157 da LC 214 (antes tinha 60% de desconto).
- Simulador do clube ganhou aviso sobre a redução de 40% para bares e restaurantes (arts. 273 a 276) e aluguel de salão ganhou ressalva; o simulador foi removido na 1.4.0.
- Notas fiscais: explicado que o Simples tem calendário próprio (emissor nacional em 01/11/2026; CBS e IBS na nota a partir de 01/01/2027).
- Novas fontes oficiais no rodapé.

## 1.1.0 · 2026-10-30 · revisão técnica

### Corrigido
- Simuladores: CBS e IBS exibidos agora somam exatamente o imposto total (o centavo que sobra vai para o IBS); no Simples, o total da opção 2 também fecha com as parcelas.
- Simuladores: campos numéricos respeitam o `max` do HTML mesmo quando o valor é digitado (percentual de vendas para empresas e alíquotas) e limitam valores absurdos, que antes viravam infinito ou NaN.
- Modo escuro: texto em destaque do bloco de exemplo e etiqueta "estamos aqui" com contraste adequado (antes cerca de 1,2:1 e 3,1:1).
- Estilos inline movidos para `style.css`, como manda o `AGENTS.md`.
- Recibo (calendário): 2027 e 2033 não dizem mais que "acabam" todos os tributos antigos; citam a exceção do IPI na Zona Franca e a permanência do Imposto Seletivo.
- Simulador do MEI: a mensagem de excesso de faturamento agora diz que o MEI deixa de ser MEI em janeiro do ano seguinte.
- `AGENTS.md`: rótulos do DAS do MEI corrigidos (R$ 86,05 é serviços; R$ 87,05 é comércio e serviços).

## 1.0.0 · 2026-10-30 · lançamento

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
- Conteúdo revisado contra fontes oficiais: alíquota de referência (teto legal de 26,5%, afirmação posteriormente superada na 1.2.0; estimativas entre 26,5% e 28%), regras do MEI, motivo do monitoramento do Pix, clubes e Imposto de Renda.
- Tabelas do MEI e do clube escondiam a coluna "Com a reforma" no celular; agora viram cartões empilhados.
- Texto cortado nas opções do seletor do simulador de clube.
