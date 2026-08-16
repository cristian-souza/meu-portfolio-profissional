# Instauro — Guia de Identidade Visual
### Documentação de marca, extraída da validação de naming (framework de 6 camadas)

---

## Status deste documento

Este guia parte de **Instauro**, nome aprovado em 5 das 6 camadas de validação automatizável (ver `validacao-nome-instauro.md`). As decisões de cor, tipografia e símbolo abaixo são uma **proposta de direção**, não uma marca registrada — os itens da seção 5 daquele documento (domínio, INPI, redes sociais) ainda são pré-requisitos antes de qualquer aplicação comercial real.

---

## 1. Símbolo

**Conceito:** quatro barras verticais em altura crescente, saindo de uma base comum.

Duas leituras se sobrepõem de propósito:
- **Leitura conceitual:** "erguer, estabelecer, construir sobre uma base" — tradução visual direta da raiz *staur-* do nome.
- **Leitura técnica:** barra de progresso / gráfico de build-deploy — ponte com o vocabulário do público-alvo (devs).

Isso não é coincidência forçada: o significado técnico só funciona porque o significado etimológico já existia primeiro. Se o símbolo funcionasse *só* como analogia de dev, seria genérico — dezenas de marcas de infra usam barra de progresso. O que sustenta a escolha é a dupla leitura.

**Arquivo:** `instauro-logo.svg`

**Regras de uso:**
- Espaço de respiro mínimo ao redor do símbolo = altura da barra mais alta.
- Tamanho mínimo de aplicação: 24px de altura (abaixo disso, usar o monograma).
- Não distorcer a proporção das barras entre si — a progressão de altura é a mensagem; achatar ou espremer o símbolo quebra a leitura.
- Não aplicar em fundos que reduzam o contraste do verde-teal abaixo de 4.5:1 (ver seção 3, acessibilidade).

**Fundo/uso incorreto a evitar:** rotacionar o símbolo, adicionar gradiente ou sombra, ou reduzir para menos de 4 barras — o número quatro não é arbitrário, mas também não carrega significado simbólico específico (não é "os quatro elementos" nem nada do tipo). É simplesmente a quantidade que melhor comunica "progressão" sem virar um gráfico de barras genérico de 6+ colunas.

---

## 2. Monograma

Versão reduzida para contextos onde o símbolo de 4 barras não cabe ou perde legibilidade: favicon, avatar de rede social, ícone de app.

**Conceito:** a letra minúscula "i" isolada (inicial de Instauro), mantendo o pingo como elemento distintivo — funciona como assinatura mínima sem tentar recriar as quatro barras em miniatura (o que ficaria ilegível em 16–32px).

**Arquivo:** `instauro-monograma.svg`

**Quando usar o monograma em vez do símbolo completo:** favicon de navegador, ícone de app mobile, avatar de redes sociais, contextos abaixo de 32px.

---

## 3. Cores

| Papel | Cor | Hex | Uso |
|---|---|---|---|
| **Primária** | Verde-teal | `#0F6E56` | Símbolo, links, CTAs primários, destaques |
| **Texto/base escura** | Verde quase-preto | `#0A2E27` | Texto principal, fundo de seções escuras |
| **Fundo neutro** | Off-white quente | `#F7F5F0` | Fundo padrão de página (não branco puro — reforça o tom institucional/atemporal) |
| **Neutro médio** | Cinza-verde | `#4A4A47` | Texto secundário, legendas |
| **Neutro claro** | Cinza-verde claro | `#D8D6D0` | Bordas, divisores, fundos de card |
| **Branco puro** | — | `#FFFFFF` | Reservado a texto sobre fundo escuro/primário — evitar como fundo geral da página |

**Por que essa paleta:**
- O verde-teal foge do azul genérico de SaaS/startup e do verde "sustentabilidade" batido — mas ainda comunica crescimento, o que está alinhado à raiz semântica do nome (renovar, estabelecer).
- O fundo off-white (em vez de branco puro `#FFFFFF`) é proposital: branco puro empurra a identidade para o registro "app moderno genérico"; o tom quebrado reforça o peso institucional que a tipografia serifada também carrega.
- **Não há cor de acento secundária definida ainda** (ex.: terracota, que apareceu como direção alternativa na exploração de "Ciclo" — ver seção 6 do documento de validação). Recomendo manter a paleta monocromática (teal + neutros) até haver necessidade real de uma segunda cor funcional (ex.: estados de erro/sucesso em produto) — adicionar cor de acento sem essa necessidade é decisão estética sem propósito.

**Acessibilidade:** `#0F6E56` sobre `#F7F5F0` passa em contraste AA para texto grande/UI (~4.6:1); para texto de parágrafo em corpo pequeno, prefira `#0A2E27` sobre `#F7F5F0` (contraste bem acima do mínimo).

---

## 4. Tipografia

| Papel | Fonte recomendada | Fallback | Uso |
|---|---|---|---|
| **Wordmark / títulos grandes** | Serifada institucional (ex.: *Fraunces*, *Source Serif 4*, *Lora*) | Georgia, serif | Logotipo textual, H1, headlines de marketing |
| **Corpo / UI** | Sans-serif técnica (ex.: *Inter*, *IBM Plex Sans*) | -apple-system, sans-serif | Parágrafos, navegação, botões |
| **Código / CLI** | Monoespaçada (ex.: *IBM Plex Mono*, *JetBrains Mono*) | ui-monospace, monospace | Blocos de código, terminal, exemplos de comando |

**Por que serifada no wordmark:** o nome "Instauro" é curto, incomum e não se explica sozinho na primeira leitura (ao contrário de "Genesis" ou "Origin", que foram descartados justamente por já *serem* óbvios demais e por isso ocupados). A serifa compensa isso — empresta peso de "fundação" mesmo antes do significado ser explicado, reforçando o próprio sentido raiz da palavra (*instaurare*, "estabelecer"). Uma sans-serif geométrica no wordmark deixaria o nome parecendo apenas mais uma startup de nome estranho gerado por IA — o oposto do que a validação tentou evitar (ver Insight 1 do documento de metodologia sobre saturação de nomes por IA).

**Por que sans técnica no corpo:** o público é dev — legibilidade em tela e neutralidade importam mais que personalidade na UI do produto em si. A personalidade fica concentrada no wordmark e no símbolo.

**Por que monoespaçada dedicada ao contexto de código:** reforça a aplicação prática do nome como comando de terminal (ver seção 5).

---

## 5. Voz e aplicação — o comando de terminal

"Instauro" funciona como verbo de ação em primeira pessoa do latim ("eu estabeleço/erijo") — o que se traduz naturalmente para um comando:

```
$ instauro init
$ instauro build
```

Essa aplicação não é decorativa: é o teste mais direto de que o nome "funciona" para o público técnico-alvo. Um nome que soa estranho como comando de CLI provavelmente vai soar estranho no dia a dia de quem o usa.

**Recomendação de tom de voz geral (site, docs, mensagens de erro/sucesso do produto):**
- Direto, sem jargão de marketing inflado — coerente com o próprio processo de validação que gerou o nome.
- Tom levemente formal é aceitável e esperado (o nome carrega isso), mas não deve virar burocrático — a ressalva já registrada na camada 5 da validação (leve tom jurídico/institucional de "instaurar um inquérito") é um risco real a monitorar, não só um detalhe.
- Evitar qualquer tentativa de "explicar" o significado latino do nome de forma forçada na home — se o nome precisar de um parágrafo de justificativa para fazer sentido, o problema não se resolve com mais texto.

---

## 6. O que ainda está em aberto

Para manter a mesma honestidade do processo de validação:

- **Cor de acento secundária:** não definida (ver seção 3).
- **Direção "Ciclo" e "Síntese"** (arco terracota, combinação arco+barras) exploradas no documento de validação seguem como alternativas não descartadas, mas não desenvolvidas aqui — este guia assume a direção "Construção" (barras) como a escolhida.
- **Domínio, INPI, redes sociais:** seguem pendentes de checagem manual — nenhuma aplicação pública desta identidade deveria acontecer antes disso.

---

*Documento gerado a partir do processo de identidade visual para Instauro, dando sequência à validação de nome (framework de 6 camadas) — para Cristian Souza, desenvolvedor fullstack.*
