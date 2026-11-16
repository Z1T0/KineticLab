# KINETIC // LAB — Roteiro do teste de usabilidade

> **16/11:** este roteiro ainda não foi aplicado com pessoas reais. A primeira versão serviu de base para um percurso cognitivo com 5 perfis simulados por IA, registrado em [08-avaliacao-simulada.md](08-avaliacao-simulada.md). Em 16/11 o roteiro foi revisado: recrutamento com filtro, facilitação por mim ou com gravação, tarefa 1 com a pergunta do número, tarefa 3 sem a dica, pergunta final aberta, termo de consentimento e critério de gravidade.

Teste no protótipo do Figma pelo celular, cerca de 15 minutos por pessoa. Duas pessoas já mostram problemas grosseiros; com cinco dá para ver se a hesitação se repete. Com qualquer um dos dois números, o resultado aponta problemas e não "valida" o produto.

## Quem recrutar
O público do brief são corredores de 24 a 45 anos que compram online. Antes de marcar, faça estas perguntas e só siga com quem responder sim às três:
1. Você corre pelo menos 2 vezes por semana?
2. Já comprou tênis de corrida pela internet?
3. Já comprou um tênis (ou outro calçado) online e o tamanho não serviu?

Não podem participar familiares, colegas próximos ou quem já viu as telas. Onde procurar: grupos de corrida de Teresina e clubes do Strava.

## Quem facilita
Eu facilito, de preferência ao lado da pessoa. Se não der para estar junto, a pessoa faz o teste sozinha, grava a tela e o áudio pelo celular e me manda o vídeo. Ninguém mais aplica o roteiro: um facilitador sem treino tende a ajudar, explicar e confirmar, e isso estraga o resultado.

## Consentimento (ler antes de começar)
"Este é um teste de um site de estudo, para o meu portfólio. Vou gravar a tela do celular e a sua voz enquanto você usa o protótipo, só para eu rever depois o que aconteceu. A gravação fica comigo, não vai ser publicada nem enviada a ninguém, e eu apago em até 30 dias. No estudo de caso você aparece sem nome, como P1 ou P2. Você pode parar a qualquer momento, sem explicar o motivo, e pedir que eu apague o que foi gravado. Tudo bem para você?"

Só comece com um sim. Se a pessoa não quiser gravar, anote à mão.

## Antes de começar (fale assim)
"Estou testando o site, não você. Não existe resposta errada. Vá falando em voz alta o que pensa enquanto usa. Se travar, tudo bem, isso me ajuda a achar o problema."

## Cenário
"Você corre umas 3 vezes por semana e seu tênis já está gasto. Um amigo indicou a KINETIC."

## Tarefas
| # | Tarefa (leia em voz alta) | Concluiu quando… |
|---|---|---|
| 1 | "Descubra qual tênis e qual tamanho a KINETIC recomenda para você." Quando a pessoa chegar na recomendação, pergunte: "Que número você compraria? Por quê?" | Chega na recomendação e diz um número. Anote se é o recomendado e o motivo que ela deu |
| 2 | "No fim de semana você vai correr numa trilha. Troque a sola para a de trilha e adicione uma palmilha." | Solado Trail Lug selecionado e palmilha na sacola |
| 3 | "Finalize a compra." Depois do pedido confirmado, com o celular virado para baixo: "Quanto você pagou de frete? E se o tênis não servir, o que acontece?" | Diz o frete e a troca em 30 dias sem voltar às telas |

A tarefa 2 usa as palavras da interface ("sola", "palmilha"). Ela mede se a pessoa acha os controles, e não se ela pensaria sozinha em trocar a sola.

Depois de cada tarefa, pergunte: "De 1 a 7, quanto foi fácil fazer isso?" (1 = muito difícil, 7 = muito fácil).

**Não ajude.** Se a pessoa perguntar, devolva: "O que você faria se eu não estivesse aqui?"

## O que anotar por tarefa
| Pessoa | Tarefa | Concluiu? (sim / com ajuda / não) | Facilidade (1 a 7) | Tempo | Onde hesitou | O que disse |
|---|---|---|---|---|---|---|
| P1 | 1 (número: ___) | | | | | |
| P1 | 2 | | | | | |
| P1 | 3 | | | | | |
| P2 | 1 (número: ___) | | | | | |
| P2 | 2 | | | | | |
| P2 | 3 | | | | | |

"Com ajuda" quer dizer que eu dei qualquer pista além de repetir a tarefa.

## Perguntas finais
1. De 1 a 5, quanto você confiaria no tamanho recomendado?
2. Teve alguma palavra que você não entendeu?
3. O que te faria desistir da compra?
4. Como você se sentiria comprando um tênis com peças trocáveis? (Depois de perguntar, espere. Não sugira palavras.)

## Como os achados viram decisão
Cada problema observado ganha uma gravidade:
- **Alta:** impede concluir a tarefa ou leva a pessoa a escolher um tamanho errado.
- **Média:** atrasa, gera dúvida ou faz a pessoa pedir ajuda.
- **Baixa:** incomoda, mas não muda o resultado.

Problema alto entra na próxima iteração mesmo que apareça em uma pessoa só. Problema médio entra quando aparece em 2 pessoas ou mais; com uma só, fica anotado para o próximo teste. Problema baixo vai para a lista de depois. Depois do teste, comparo o que as pessoas fizeram com o que o percurso simulado previu e publico os dois lado a lado no case.

## Como abrir o protótipo (antes de chamar a pessoa)
1. No Figma, abra a página **09 · Protótipo**. No painel **Prototype** (à direita, sem nada selecionado), em **Device**, escolha um iPhone de 390 × 844 (iPhone 13, 14 ou 15).
2. Abra o link no celular, com o app do Figma ou o navegador:
   https://www.figma.com/proto/WHFA16vy2gCG04ZnnqaNjX/?node-id=35-18&starting-point-node-id=35%3A18&scaling=scale-down-width&content-scaling=fixed
3. Faça as 3 tarefas uma vez antes do teste. Depois volte para a Home: pressione **R** no computador, ou toque com dois dedos no celular e escolha "Restart".

## O que funciona no protótipo
- **Tarefa 1:** botão "Encontre seu ajuste" → 5 perguntas → Recomendação. Nos passos 1, 3, 4 e 5, tocar numa opção já avança (o Continuar também funciona). **O passo 2 é diferente (mudou em 15/11):** a pessoa marca o número (34 a 45) e a largura do pé e toca em Continuar. A tela rola. Na recomendação, "Amortecimento" e "Resposta" trocam a entressola entre Stable e Pulse, e o total muda.
- **Tarefa 2:** na página do produto, o chip Trail Lug troca o solado e "+ Adicionar" na palmilha marca como adicionada. A sacola mostra a combinação escolhida. Também dá para adicionar a palmilha pela sacola.
- **Tarefa 3:** "Finalizar compra" → Checkout, com frete e garantia visíveis → "Pagar" → **tela do Pix** (nova em 15/11) → "Copiar código Pix" → "Código copiado" → o pedido confirma sozinho em alguns segundos. A aba "Cartão" abre o formulário, e a recusa só aparece depois de "Pagar".

**Limites:**
- O checkout sempre mostra os 2 itens (R$ 1.788), mesmo que a pessoa não tenha adicionado a palmilha. Se isso acontecer, anote que a tarefa 2 não foi concluída.
- No passo 2, dá para marcar mais de um número ou mais de uma largura (a marcação é só visual). Se acontecer, anote.
- Na página do produto, os tamanhos agora marcam e desmarcam ao toque, mas o preço e a sacola não mudam.

**Mudou em 16/11 (não é mais limite):** quem escolhe "Resposta" (Pulse) na recomendação chega à página do produto com a Pulse marcada e R$ 1.799, e a sacola, o checkout, o Pix e o pedido confirmado somam R$ 1.988 com a palmilha. O hodômetro do pedido confirmado usa a faixa marcada no passo 3. Se a pessoa testar a Pulse, confira se os totais batem e anote se não baterem.

**O que observar a mais (mudanças de 15/11):**
- No passo 2, a pessoa entende "largura do pé"? Sabe responder?
- Na recomendação, ela nota o "Seu foco"? Entende a diferença entre amortecimento e resposta?
- Na tela do Pix, ela entende que precisa ir ao app do banco?
