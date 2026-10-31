# AGENTS.md

Orientações para agentes de IA (e pessoas) que trabalham neste repositório.

## O que é

**RESET tributário** (Reforma Explicada Sem Enrolação Tributária): site estático em português do Brasil que explica a reforma tributária (EC 132/2023, LC 214/2025, LC 227/2026) para leigos. Foco: MEI, Pix, clubes e associações, preços e prazos de 2026 a 2033.

- Repositório: https://github.com/luizcoura/reset-tributario
- Site: https://luizcoura.github.io/reset-tributario/ (GitHub Pages, publicado a partir de `main`, pasta raiz)
- Licença: MIT

## Estrutura

| Arquivo | Função |
|---|---|
| `index.html` | Página principal: texto, calendário e 4 simuladores em abas (consumidor, MEI, Simples Nacional, Pix), com script inline no fim. O `<head>` tem a tag `google-site-verification` do Search Console: não remova |
| `perguntas.html` | Perguntas frequentes, com respostas curtas e links para a página principal |
| `style.css` | CSS único das duas páginas (tokens de cor, modo escuro, recibo, tabelas, abas, FAQ) |
| `og-image.png` | Imagem de pré-visualização 1200×630 |
| `favicon.svg`, `favicon-48.png`, `apple-touch-icon.png` | Ícones |
| `sitemap.xml`, `robots.txt` | SEO |
| `CHANGELOG.md` | Histórico de mudanças |

Não há build, dependências nem framework. Para ver localmente, abra `index.html` no navegador.

Fontes novas vão na lista "Fontes consultadas" no rodapé do `index.html`, com a data de publicação que aparece na página (ou "sem data visível"); a lista é ordenada por essa data, da mais recente para a mais antiga, em dois grupos (oficiais; imprensa e entidades). Texto com número ou regra nova linka a fonte no próprio parágrafo.

## Regras

- **Idioma:** todo texto do site, commits e documentação em português do Brasil.
- **Público:** leigo. Frases curtas, sem jargão sem explicação. Termos técnicos entram no glossário.
- **Escrita para leigo:** (1) a primeira frase de cada bloco responde "e eu com isso?"; lei, artigo, data e fonte vêm depois, no fim do bloco ou numa nota pequena. (2) No máximo 25 palavras por frase e 3 números por parágrafo; passou disso, vira lista ou tabela. (3) Toda sigla é escrita por extenso ou explicada na primeira vez em cada página (use `<abbr title="...">`), e todo termo técnico (crédito, regime regular, desenquadramento, imunidade) tem verbete no glossário. (4) Um nome só para cada coisa em todo o site: "regime regular" (para pagar CBS e IBS à parte, como as empresas comuns), "guia do Simples (DAS)", "guia fixa do MEI (DAS-MEI)", "empresa cliente". (5) Rótulo de campo é uma pergunta em linguagem comum, com exemplo em letra pequena. (6) Mantenha as ressalvas ("em regra", "depende da regulamentação"), mas só uma por parágrafo.
- **Conteúdo tributário:** só afirme o que tem fonte (Planalto, Receita Federal, Ministério da Fazenda, Agência Senado). Quando depender de regulamentação, diga isso no texto em vez de afirmar. Os simuladores são estimativas didáticas, não cálculo oficial. Prefira fonte primária (texto da lei ou do ato) a notícia ou blog: já erramos por confiar em fonte secundária desatualizada (Fenacon com salário mínimo de R$ 1.627 antes do decreto, Contábeis com prazo antigo, Simtax chamando 26,5% de teto). Notícia atualizada recentemente não prova que o ato citado nela está em vigor.
- **Pontos pouco confirmados** (manter com ressalva, e conferir em fonte primária quando der): parcela de CBS e IBS dentro da guia do Simples e alíquota efetiva (valores de exemplo na aba Simples); janelas de opção do Simples (Resolução CGSN 194: Simples até 15/10, regime regular até 30/10, cancelamento de 03/11 a 20/12/2026, conforme notícias da Fazenda e da Receita; a nova janela de abril vem só da página Reforma de Fato, sem norma conferida); limites de R$ 5 mil e R$ 15 mil da e-Financeira (o ato da nota, IN 2.219/2024, consta como revogado pela IN 2.247/2025; não há ato posterior conferido, então o site não os afirma como regra em vigor); lista do IPI residual (o TCU diz que ainda não tem definição); categorias dos simuladores (alimento, educação, saúde, remédio dependem das listas dos anexos da LC 214); PIS/Cofins de associações e Simples de associações ("em regra"); texto do art. 6º, XII da LC 214 (lido só por fontes secundárias); condições de sociedades no art. 127 (profissional liberal). Já conferidos em fonte primária: Lei 15.270/2025 (dividendos e imposto mínimo, lida no Planalto), cashback do art. 118 e lista do art. 127 (lidos por busca e por revisão independente, não por inteiro no Planalto).
- **Data de conferência:** sempre que mudar ou revisar o conteúdo, atualize "Conteúdo conferido em ..." no rodapé do `index.html` e o `lastmod` da página alterada no `sitemap.xml`.
- **Alíquota:** cálculo "por fora". O imposto embutido no preço é `preço × r / (1 + r)`. Nos simuladores a alíquota tem dois campos, CBS 11,3% (proposta do TCU de 28/10/2026 para 2027, sujeita ao Senado até 15/12, segundo a imprensa; a página do TCU não cita esse prazo) e IBS 18,7% (projeção), somando cerca de 30%; 26,5% é a referência legal (acima disso, o governo deve propor redução ao Congresso, sem trava automática) e a estimativa antiga do governo era CBS 8,8% + IBS 17,7%. Atualize quando o Senado decidir. O cálculo usa a soma e divide o resultado entre CBS e IBS na proporção das alíquotas.
- **MEI 2026:** DAS de R$ 82,05 (comércio/indústria), R$ 86,05 (serviços) e R$ 87,05 (comércio e serviços), limite de R$ 81 mil (o PLP 186/2026, sancionado em 21/10/2026, eleva para R$ 110 mil em 2027 e R$ 140 mil em 2028). O salário mínimo de 2026 é R$ 1.621 (Decreto 12.797/2025, notícia da Receita de 02/01/2026); a DAS é 5% disso mais R$ 1 de ICMS e/ou R$ 5 de ISS. No ano de abertura, o limite é proporcional (R$ 6.750 por mês de atividade), e passar de 20% faz a saída valer desde a abertura ou desde janeiro. Atualize se o salário mínimo mudar.

## Estilo e CSS

- Todo CSS vai em `style.css`; não volte a colocar estilo inline nas páginas.
- Cores via variáveis em `:root` (`--papel`, `--tinta`, `--carimbo`, `--verde`), com redefinição para modo escuro.
- Tabelas de comparação viram cartões em telas até 40rem (`td:nth-of-type(1)::before` = "Hoje", `(2)` = "Com a reforma"). Mantenha duas colunas de dados nessas tabelas ou ajuste esse CSS.
- Respeite `prefers-reduced-motion`, foco visível no teclado e abas com ARIA.

## Ao mudar algo

1. Nova página: adicione ao `sitemap.xml`, ao menu e ao rodapé; use canonical, Open Graph e JSON-LD como as existentes.
2. Mudou título ou texto principal: regenere o `og-image.png` (HTML renderizado no Chrome headless, redimensionado com `sips`).
3. Teste em tela larga e em 390px, nos modos claro e escuro, e navegue pelas abas com o teclado. Dicas: o escuro vem de `prefers-color-scheme`, então para ver o claro ponha `data-theme="light"` no `<html>`; para 390px use um iframe de 390px de largura (a janela do Chrome não passa de 500px); para conferir o site publicado, abra com `?v=<hash do commit>` para fugir do cache.
4. Registre no `CHANGELOG.md` com uma nova versão e atualize a linha "Versão X.Y.Z" no rodapé do `index.html` e do `perguntas.html`. A regra da numeração está no topo do `CHANGELOG.md`.
5. Teste os simuladores nos casos de borda, não só no padrão: taxas de CBS/IBS zeradas (as duas, só uma), meses de atividade fracionados ou fora de 1 a 12, MEI exatamente 20% acima do limite, crédito maior/menor/igual e saldo credor no Simples. Confira que o resumo e as mensagens não afirmam crédito sem a condição "se a compra der direito a ele".
6. Revisão independente: peça a outro agente (por exemplo, o Codex no Maestri) para revisar o site publicado com `?v=<hash>`, somente leitura, usando fontes primárias. Cada rodada achou erros novos, às vezes introduzidos pela correção anterior; releia o diff antes de publicar.
7. Commit em português, no imperativo, com mensagem curta (ex.: "Adiciona página de perguntas frequentes"). O push publica o site; espere o build do Pages antes de conferir.

## Fora do escopo

Não há backend, formulários, cookies nem rastreamento. Não adicione scripts de terceiros sem pedido explícito.
