# KINETIC // LAB · Aderência ao brief, item por item (15/11)

Reli o PDF "Estudo de Caso UX/UI – KINETIC // LAB" seção por seção e conferi cada pedido contra o Figma (páginas 01 a 11), os documentos e o estudo de caso. Não confiei no diário: abri as telas.

Legenda: ✅ atendido · 🟡 atendido em parte ou com desvio justificado · 🔧 corrigido hoje · ⏳ fica para depois do teste

## 1. Conceito

| Pedido do brief | Status | Onde está / o que fiz |
|---|---|---|
| Plataforma modular: cabedal, entressola e solado trocáveis | ✅ | Produto KINETIC M1 (00-escopo.md), Fig. 01 "vista explodida" |
| Problema: 68% do abandono vem de dúvida de tamanho e de densidade da espuma | 🔧 | A densidade já era tratada (pisada + peso → entressola). O tamanho era o ponto fraco: o passo 2 foi refeito (ver 2.1) |
| Oportunidade: configurador simples, menos devolução, LTV com refis e venda cruzada (palmilha, meia, sensor) | ✅ | Refil de R$ 349, hodômetro estimado no pedido confirmado, os 3 acessórios na PDP e na sacola |
| Público de 24 a 45 anos, rua, ultra, trilha e treino híbrido | ✅ | Personas Renata (maratona) e Diego (rua + trilha, ultra de 50 km). Mosaico "Híbrido" na Home |
| Dores: acertar tamanho sem provar, troca burocrática, desgaste em 400–600 km | ✅ | Passo 2 + troca grátis em 30 dias + refil a cada 600 km |

## 2. Inovações de UX/UI

### 2.1 Questionário de ajuste ("Biometric Fit & Stride Matcher")

| Pedido | Status | Onde está / o que fiz |
|---|---|---|
| Nome | 🟡 desvio | Virou "Encontre seu ajuste": não há biometria, é questionário (decisão de 15/11) |
| Coleta tipo de pisada | ✅ | Passo 1, com "Não sei" |
| Coleta peso aproximado | ✅ | Passo 5, por faixa, com "Prefiro não dizer" |
| Coleta volume semanal | ✅ | Passo 3 |
| Coleta foco: amortecimento x responsividade | 🔧 | **Não era perguntado.** Entrou como "Seu foco" no topo da recomendação (Stable x Pulse, com o preço). Não virou 6º passo porque a CSD supõe abandono acima de 5 passos. O conflito aparece na tela: pisada pronada pede Stable, resposta pede Pulse |
| Recomenda a densidade exata da entressola | ✅ | Recomendação com o motivo de cada peça |
| Recomenda tamanho "com base na anatomia do pé" | 🔧 | **Só perguntava o número (36, 37 ou 38).** Passo 2 agora tem grade de 34 a 45 e largura do pé (fino, médio, largo). A recomendação cita os dois: "Pé largo? Aí sugerimos subir um número" |
| (achado extra) Recomendação citava dados não perguntados | 🔧 | "Manhã cedo em São Paulo" e "50 km por semana" saíram, no mobile e no desktop |
| (achado extra) "Por que perguntamos?" dos passos 2 a 5 | 🔧 | Estava oculto e era cópia do passo 1. Cada passo agora tem o seu texto |

### 2.2 Configurador ("3D Modular Footwear Builder")

| Pedido | Status | Onde está |
|---|---|---|
| Visualizador 3D interativo | 🟡 desvio | Vista explodida em camadas, que acende a peça trocada. O 3D completo ficou como evolução (decisão de 15/11: peso no celular) |
| Cabedal: malha ultraleve, ripstop, membrana impermeável | ✅ | Aero Knit, Ripstop (+R$ 120), Storm (+R$ 240) |
| Entressola: densidades e drop de 4 a 10 mm | ✅ | Ground 4, Pulse 6, Flow 8, Stable 10 mm, com "O que é drop?" |
| Solado: cravos para terra/lama; borracha para asfalto molhado | ✅ | Trail Lug 5 mm; Road Grip |

### 2.3 Frete e custo por km

| Pedido | Status | Onde está / o que fiz |
|---|---|---|
| Prazo e valor do frete na PDP | ✅ | Bloco "Frete e prazo" com CEP validado |
| "Via detecção de localização ou CEP rápido" | 🔧 | Só havia CEP. Entrou "Usar minha localização" na PDP mobile (UI e 4 estados do protótipo) e desktop |
| Gráfico comparando custo por km com modelos descartáveis | ✅ | Componente "Custo por km": R$ 1,28 x R$ 2,17, 41% a menos |
| Gráfico "dinâmico" | 🟡 | O valor não muda com a configuração (com a Pulse seria R$ 1,39/km). Fica anotado como regra para o desenvolvimento |

## 3. Requisitos funcionais

| Pedido | Status | Onde está / o que fiz |
|---|---|---|
| Filtros: terreno, pisada, quilometragem, compatibilidade | ✅ | Catálogo: Trilha, Pisada, Km por semana, "Encaixa no M1" |
| Cross-sell contextual na PDP e no carrinho | ✅ | Sacola muda conforme o solado ("Combina com seu Trail Lug") |
| Exemplo do brief: solado de trilha → meia anti-atrito e palmilha de impacto | ✅ | Sacola Trail Lug sugere exatamente esses dois |
| Checkout em etapa única | ✅ | Mobile e desktop |
| Endereço de entrega = cobrança com um toque | ✅ | "Usar o mesmo endereço para cobrança", marcado |
| Cartão tokenizado | 🟡 | Aba Cartão e "Compra segura". A palavra "token" não aparece para o cliente, e acho certo: é detalhe técnico |
| Pix com QR Code instantâneo | 🔧 | **A tela não existia** (o checkout dizia "o QR aparece depois de confirmar"). Nova tela do Pix: "Copiar código Pix" em destaque (no celular ninguém lê o QR da própria tela), QR para outro aparelho, validade do código, "nada é cobrado antes de confirmar". Ligada no protótipo: Pagar → Pix → Pedido confirmado |
| Apple Pay e Google Pay | ✅ | "Pagamento expresso" no topo do checkout |
| Selo "30 dias de teste de corrida ou devolução grátis" | ✅ | PDP, sacola, checkout e Home |

## 4. Roteiro do portfólio (fases e entregáveis)

| Pedido | Status | Onde está / o que fiz |
|---|---|---|
| Matriz CSD | ✅ | 01-descoberta.md e Figma p. 02 |
| Benchmarking com marcas de ponta | 🟡 | O benchmarking compara padrões de mercado, sem nomear marcas. O brief fala em "marcas de ponta": se der tempo, vale citar 2 ou 3 lojas reais no case |
| Roteiro de entrevistas com corredores **e especialistas biomecânicos** | 🔧 | Só havia o roteiro dos corredores. Incluí o roteiro do especialista em 01-descoberta.md |
| 2 personas, mapa de empatia, jornada com fricções | ✅ | Renata e Diego; empatia da Renata; jornada com 7 fricções (simuladas e sinalizadas) |
| Sitemap e user flow | ✅ | Figma p. 04 |
| Wireframes das 4 telas (Home, Catálogo, PDP, Checkout) | ✅ | Figma p. 05 (7 telas) |
| Design system: tipografia, cores, componentes | ✅ | Figma p. 06 |
| Protótipo navegável com microinterações | ✅ | Figma p. 09 (agora com 20 telas e estados: entraram a recomendação com Pulse e o Pix) |
| Telas mobile **e desktop** com estados de erro, foco e sucesso | 🟡 | Mobile tem os três. Desktop tem foco (celular) e sucesso (CEP), mas não tem erro nem a tela de catálogo. Fica como lacuna conhecida |
| Narrativa do case com **impacto estimado em conversão** | 🔧 | O case não tinha essa parte. Criei o 07-plano-de-medicao.md (metas, eventos, fórmulas, guardrails e um cenário de impacto marcado como estimativa) e a seção correspondente no case |

## 5. Métricas e KPIs

| Meta do brief | Status | Onde está |
|---|---|---|
| Conversão do checkout de 1,8% para 3,2% | 🔧 | Estava só na p. 01. Agora tem evento, fórmula e guardrail no 07-plano-de-medicao.md |
| Devolução por tamanho de 22% para menos de 6% | 🔧 | Idem. Depende do passo 2 novo |
| Uso do configurador acima de 45% | 🔧 | Idem |
| Tíquete médio +25% com combos (segundo solado, palmilha) | 🟡 ⏳ | Palmilha ok. O **segundo solado** só é oferecido no desktop. Na PDP mobile, o card "Solado Trail Lug + Adicionar" competiria com a tarefa 2 do teste (trocar o solado), então entra depois do teste |

## 6. Teste de usabilidade

| Pedido | Status | Observação |
|---|---|---|
| Tarefa 1: calibrar o tênis pelo questionário | ✅ | |
| Tarefa 2: trocar para o solado de **chuva** e incluir palmilha | 🟡 desvio | No projeto, a recomendação já entrega o Road Grip (o solado de chuva). Pedir para trocá-lo não testaria nada, então a tarefa virou "trocar para o de trilha". Decidido em 15/11 |
| Tarefa 3: checkout conferindo frete e garantia | ✅ | |
| Métricas: conclusão, tempo, hesitação | ✅ | Tabela em 02-roteiro-teste.md |

## 7. MVP x V2

| Pedido | Status |
|---|---|
| MVP: questionário, PDP com troca, carrinho lateral com frete e cross-sell, checkout em tela única | ✅ |
| V2: escaneamento do pé com câmera; Strava/Garmin para o refil | ✅ marcados como V2 (sem aparecer "V2" para o cliente, corrigido hoje) |

## 8. UX writing

| Pedido | Status | Onde está |
|---|---|---|
| "Teste por 30 dias na corrida. Troca ou devolução 100% gratuita sem burocracia" | ✅ | "30 dias de teste na corrida. Não gostou? Troca ou devolução grátis, sem burocracia." |
| "1 base + 3 refis = 1.800 km, poupa 40%" | 🟡 desvio | A conta do brief não fechava. Refeita: 1 base + 2 refis = 1.800 km, 41% a menos (00-escopo.md) |
| Indicadores sutis de criptografia; preenchimento com carteira digital | ✅ | "🔒 Compra segura" no topo do checkout; Apple Pay e Google Pay |
| Linguagem do brief em português de Portugal | 🟡 desvio | Interface em português do Brasil |

## Resumo
- **Corrigido hoje (7):** foco, tamanho por anatomia, dados inventados na recomendação, "por que perguntamos?", tela do Pix, localização no frete, "V2" visível para o cliente. Também: roteiro do especialista, plano de medição e impacto estimado.
- **Desvios justificados (5):** nome do questionário, 3D → vista explodida, tarefa 2, conta dos 41%, PT-BR.
- **Em parte:** benchmarking sem marcas, cartão tokenizado sem menção, gráfico de custo por km que não muda.
- **Lacunas conhecidas:** segundo solado na PDP mobile (depois do teste), estado de erro e catálogo no desktop, custo por km que não muda com a configuração, tela de medição com folha A4.
