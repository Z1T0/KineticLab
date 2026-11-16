# KINETIC // LAB · Percurso cognitivo com 5 perfis simulados (15/11)

> **Nota de 16/11:** o nome certo para o que está aqui é percurso cognitivo com perfis simulados por IA. Serve para achar falhas de lógica no protótipo e não mede comportamento de gente. As notas de confiança, as contagens de "concluíram" e as falas abaixo foram inventadas para cada perfil e não são dados; no estudo de caso ficaram só os problemas de lógica. O perfil "Diego, 31" foi renomeado para Caio, para não confundir com a persona Diego, 29, da descoberta.

**Isto é uma simulação feita com IA.** Sem tempo para recrutar corredores, percorri o protótipo mobile no Figma com ajuda de IA no papel de 5 perfis fictícios. Cada perfil seguiu um caminho diferente. As falas são simuladas. Nenhuma pessoa real usou o produto; o teste com pessoas é o próximo passo.

Não confundir com [05-avaliacoes.md](05-avaliacoes.md): lá, 5 avaliadores simulados (recrutadora, head de design, especialista em acessibilidade etc.) leram o projeto inteiro. Aqui, 5 compradores simulados fizeram as 3 tarefas do [roteiro de teste](02-roteiro-teste.md) no protótipo.

Figma: página **10 · Avaliação simulada** (método, perfis, resultados, achados) e página **11 · Iteração**, prancha "Iteração 1 · Depois da avaliação simulada".

## Tarefas
1. "Descubra qual tênis e qual tamanho a KINETIC recomenda para você."
2. "No fim de semana você vai correr numa trilha. Troque a sola para a de trilha e adicione uma palmilha."
3. "Finalize a compra. Antes de pagar, confira o frete e a garantia."

## Perfis (fictícios)
| Perfil | Quem é | Caminho no protótipo | Confiança no tamanho | Fala simulada |
|---|---|---|---|---|
| Caio, 31 | Corre 30 km por semana, calça 42, pisada neutra, rua e trilha | Neutra → 42 e pé médio → 20 a 50 km → os dois terrenos → mais de 80 kg → recomendação → Trail Lug + palmilha → Pix | 1 de 5 | "Marquei 42 e ele manda eu ficar no 37?" |
| Lúcia, 47 | Corre há 3 meses, não sabe a pisada nem o número de corrida | "Não sei" na pisada → "Me ajude a medir o pé com uma folha A4" | 3 de 5 | "Disse que ia descobrir com duas perguntas. Que perguntas?" |
| Marcos, 44 | Maratonista, compara preço | Página do produto → Trail Lug → "+ Adicionar" na palmilha → barra do total → sacola | 2 de 5 | "Adicionei a palmilha e o total não mudou. Entrou ou não?" |
| Bia, 27 | Paga tudo no cartão | Checkout → aba "Cartão" → Pix | 3 de 5 | "Recusado? Eu nem digitei o cartão." |
| Seu Paulo, 58 | Paga no Pix, lê devagar, celular pequeno | Checkout → "Pagar com Pix" → "Copiar código Pix" | 3 de 5 | "Copiei e já está pago? Nem abri o banco." |

## Resultado por tarefa
| Tarefa | Concluíram | Onde travaram |
|---|---|---|
| 1 | 5 de 5, confiança baixa | A recomendação ignora as respostas: Caio marcou 42 e neutra e leu "Você usa 37" e "pisada pronada". No "Não sei" da pisada, Lúcia não viu as 2 perguntas prometidas, e a medição com folha A4 não tem tela. Paulo não sabia o que é "M1". |
| 2 | 5 de 5, 1 com dúvida | Todos acharam o Trail Lug e a palmilha. Depois da palmilha, a barra continuou em "Configuração base · R$ 1.599"; só a sacola mostrou R$ 1.788. |
| 3 | 5 de 5 | Frete grátis e 30 dias à vista antes de pagar. A aba "Cartão" mostrou "pagamento recusado" sem nada digitado. "Copiar código Pix" levou direto ao pedido confirmado. |

Sem tempo cronometrado: numa simulação, o tempo não mede nada.

## Hipóteses do roteiro
| Hipótese | Resultado simulado |
|---|---|
| H1 · O questionário resolve a dúvida de tamanho? | Não deu para avaliar: a recomendação do protótipo dizia 37 e pisada pronada para todo mundo. O que falhou foi o protótipo; a hipótese só pode ser testada com pessoas. |
| H2 · Dá para trocar uma peça e achar um acessório sem procurar? | Sim. Um perfil duvidou se a palmilha entrou. |
| H3 · Frete e garantia aparecem antes de pagar? | Sim. |
| H4 · "Drop" atrapalha? | Inconclusivo. A IA conhece o termo; só pessoas reais respondem esta. |

## Achados
| # | Achado | Severidade | Vai para a página 11? |
|---|---|---|---|
| 1 | A recomendação ignora as respostas: diz sempre 37, pé médio, pisada pronada e asfalto. | Alta | Sim |
| 2 | O "Não sei" da pisada promete 2 perguntas que não existem. O mesmo texto aparece nos passos 3 e 4, e a medição com folha A4 não tem tela. | Alta | Sim |
| 3 | A aba "Cartão" já mostra pagamento recusado, e "Copiar código Pix" confirma o pedido sem passar pelo banco. | Média | Sim |
| 4 | O total da página do produto não soma a palmilha nem muda o rótulo "Configuração base". | Média | Sim (corrigido) |
| 5 | "M1" aparece no passo 2 sem explicação. | Baixa | Depois |
| 6 | A sacola mostra "2" na home antes de qualquer compra. | Baixa | Depois |
| 7 | "Chega quinta, 20/11": 20/11/2026 é uma sexta-feira. | Baixa | Depois |

Severidade: alta derruba uma hipótese ou impede a tarefa; média atrasa ou gera dúvida; baixa incomoda.

## O que funcionou para todos os perfis
- O aviso "Solado trocado para Trail Lug. O total continua R$ 1.599" logo depois da troca.
- A sacola com Trail Lug, palmilha no tamanho, frete grátis e R$ 1.788.
- Frete, prazo e garantia de 30 dias visíveis antes de pagar.
- A tela do Pix: valor, validade do código, QR Code para outro aparelho e "nada é cobrado antes de você confirmar".
- A tela de recusa diz que nada foi cobrado e oferece o Pix.

## Mudanças feitas no protótipo (página 11, 15/11)
1. **Respostas:** variáveis do Figma guardam número, largura, pisada e terreno. A recomendação, a página do produto e a sacola leem essas variáveis. Quem marca 42 e pé largo vê "42 · Considere subir um número".
2. **"Não sei":** duas perguntas (para que lado o tênis velho tomba e onde dói depois de correr), textos próprios nos passos 3 e 4 e a tela de medição com a folha A4, em que cada medida em cm vira um número.
3. **Pagamento:** a aba "Cartão" abre o formulário (número, validade, CVV, parcelas) e a recusa só vem depois de "Pagar"; o Pix mostra "Código copiado" e a confirmação chega sozinha 4 segundos depois.
4. **Total da página do produto:** a barra diz a configuração escolhida e o tamanho, e soma a palmilha (R$ 1.788).

Conferido no protótipo com o caminho do Caio (neutra, 42, pé largo, rua e trilha) e com o "Não sei" e a folha A4. Ainda abertos: achados 5, 6 e 7.

## Limites desta avaliação
- Uma IA sabe onde estão os botões e não se cansa. Pessoas reais travam em vocabulário, confiança na marca e pressa, que a simulação não mostra.
- Não deu para testar com leitor de tela: o protótipo do Figma não expõe nada para ele.
- As notas de confiança e as falas foram inventadas para cada perfil, a partir do que a tela mostrou no caminho dele.
