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
| `index.html` | Página principal: texto, calendário e 5 simuladores em abas (consumidor, MEI, Simples Nacional, clube, Pix), com script inline no fim. O `<head>` tem a tag `google-site-verification` do Search Console: não remova |
| `perguntas.html` | Perguntas frequentes, com respostas curtas e links para a página principal |
| `style.css` | CSS único das duas páginas (tokens de cor, modo escuro, recibo, tabelas, abas, FAQ) |
| `og-image.png` | Imagem de pré-visualização 1200×630 |
| `favicon.svg`, `favicon-48.png`, `apple-touch-icon.png` | Ícones |
| `sitemap.xml`, `robots.txt` | SEO |
| `CHANGELOG.md` | Histórico de mudanças |

Não há build, dependências nem framework. Para ver localmente, abra `index.html` no navegador.

Fontes novas vão na lista "Fontes consultadas" no rodapé do `index.html`. Texto com número ou regra nova linka a fonte no próprio parágrafo.

## Regras

- **Idioma:** todo texto do site, commits e documentação em português do Brasil.
- **Público:** leigo. Frases curtas, sem jargão sem explicação. Termos técnicos entram no glossário.
- **Conteúdo tributário:** só afirme o que tem fonte (Planalto, Receita Federal, Ministério da Fazenda, Agência Senado). Quando depender de regulamentação, diga isso no texto em vez de afirmar. Os simuladores são estimativas didáticas, não cálculo oficial.
- **Pontos pouco confirmados** (manter com ressalva): parcela de CBS e IBS dentro da guia do Simples e alíquota efetiva (valores de exemplo na aba Simples), prazos da opção pelo Simples híbrido (setembro de 2026 com cancelamento até 30/11, segundo a Fazenda; nova janela em abril, segundo a Receita; confira se houver prorrogação), associações e Simples ("em regra"), PIS/Cofins sobre mensalidade ("em geral"), redução de 30% para profissionais, percentuais do cashback, lista de remédios com alíquota zero.
- **Data de conferência:** sempre que mudar ou revisar o conteúdo, atualize "Conteúdo conferido em ..." no rodapé do `index.html` e o `lastmod` da página alterada no `sitemap.xml`.
- **Alíquota:** cálculo "por fora". O imposto embutido no preço é `preço × r / (1 + r)`. Nos simuladores a alíquota tem dois campos, CBS 11,3% (proposta do TCU de 28/10/2026 para 2027, sujeita ao Senado até 15/12) e IBS 18,7% (projeção), somando cerca de 30%; 26,5% é a referência legal (acima disso, o governo deve propor redução ao Congresso, sem trava automática) e a estimativa antiga do governo era CBS 8,8% + IBS 17,7%. Atualize quando o Senado decidir. O cálculo usa a soma e divide o resultado entre CBS e IBS na proporção das alíquotas.
- **MEI 2026:** DAS de R$ 82,05 (comércio/indústria), R$ 86,05 (serviços) e R$ 87,05 (comércio e serviços), limite de R$ 81 mil (o PLP 186/2026, sancionado em 21/10/2026, eleva para R$ 110 mil em 2027 e R$ 140 mil em 2028). Atualize se o salário mínimo mudar.

## Estilo e CSS

- Todo CSS vai em `style.css`; não volte a colocar estilo inline nas páginas.
- Cores via variáveis em `:root` (`--papel`, `--tinta`, `--carimbo`, `--verde`), com redefinição para modo escuro.
- Tabelas de comparação viram cartões em telas até 40rem (`td:nth-of-type(1)::before` = "Hoje", `(2)` = "Com a reforma"). Mantenha duas colunas de dados nessas tabelas ou ajuste esse CSS.
- Respeite `prefers-reduced-motion`, foco visível no teclado e abas com ARIA.

## Ao mudar algo

1. Nova página: adicione ao `sitemap.xml`, ao menu e ao rodapé; use canonical, Open Graph e JSON-LD como as existentes.
2. Mudou título ou texto principal: regenere o `og-image.png` (HTML renderizado no Chrome headless, redimensionado com `sips`).
3. Teste em tela larga e em 390px, nos modos claro e escuro, e navegue pelas abas com o teclado. Dicas: o escuro vem de `prefers-color-scheme`, então para ver o claro ponha `data-theme="light"` no `<html>`; para 390px use um iframe de 390px de largura (a janela do Chrome não passa de 500px); para conferir o site publicado, abra com `?v=<hash do commit>` para fugir do cache.
4. Registre no `CHANGELOG.md`.
5. Commit em português, no imperativo, com mensagem curta (ex.: "Adiciona página de perguntas frequentes"). O push publica o site; espere o build do Pages antes de conferir.

## Fora do escopo

Não há backend, formulários, cookies nem rastreamento. Não adicione scripts de terceiros sem pedido explícito.
