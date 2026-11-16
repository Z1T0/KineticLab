# KINETIC // LAB · Plano de medição e impacto estimado (15/11)

O brief pede 4 metas (seção 5) e um case com "impacto estimado em conversão" (fase 4). As metas estavam na página 01 do Figma, mas não havia como saber se o design chegou lá. Este arquivo diz o que medir, como calcular e o que não pode piorar.

> As metas vêm do brief. Os cenários de impacto no fim são **estimativas** com os números do brief. Não são resultado. O teste de 16/11 mede se as pessoas conseguem fazer as tarefas, não estas metas.

## Eventos que o site precisa registrar

| Evento | Quando dispara | Dados |
|---|---|---|
| `questionario_iniciado` | Toque em "Encontre seu ajuste" | origem (Home, PDP, menu) |
| `questionario_passo` | Cada resposta | passo (1–5), resposta, usou "Não sei"? |
| `questionario_concluido` | Chega na recomendação | entressola, tamanho e largura recomendados |
| `foco_escolhido` | Toque em Amortecimento ou Resposta | foco, entressola resultante |
| `modulo_trocado` | Troca de chip na PDP | peça, de, para, veio do questionário? |
| `tamanho_escolhido` | Adiciona à sacola | tamanho, igual ao recomendado? |
| `acessorio_adicionado` | "+ Adicionar" na PDP ou na sacola | item, onde, solado no momento |
| `frete_calculado` | CEP válido ou localização | método (CEP ou localização) |
| `checkout_iniciado` | "Finalizar compra" | valor, itens |
| `pagamento_enviado` | "Pagar" | método (Pix, cartão, carteira) |
| `pagamento_recusado` | Banco recusa | método, motivo |
| `pix_expirado` | Código passa da validade | valor |
| `pedido_pago` | Aprovação | valor, itens, método |
| `devolucao_aberta` | Cliente pede troca ou devolução | motivo (escolha única: tamanho, largura, conforto, defeito, outro), km estimados |

## As 4 metas

### 1. Conversão: de 1,8% para 3,2%
- **Fórmula:** pedidos pagos ÷ sessões. Se fosse a conversão de quem já está no checkout, 1,8% seria baixíssimo: o abandono de carrinho médio fica perto de 70%, segundo o Baymard Institute, então algo como 30% de quem chega ao carrinho compra. Por isso leio o número do brief como **conversão do site**. Vale confirmar com quem escreveu o brief.
- **Para achar onde trava:** funil `checkout_iniciado` → `pagamento_enviado` → `pedido_pago`, separado por método.
- **O que o design fez:** checkout em tela única, carteira digital no topo, frete antes do carrinho, tela do Pix com "copiar código".
- **Não pode piorar:** taxa de `pagamento_recusado` e de `pix_expirado`.

### 2. Devolução por tamanho: de 22% para menos de 6%
- **Fórmula:** devoluções com motivo "tamanho" ou "largura" ÷ pares entregues, em até 30 dias.
- **Separar sempre:** fez o questionário x não fez; comprou o tamanho recomendado x mudou. Se quem segue a recomendação devolve tanto quanto quem não segue, a recomendação não está ajudando.
- **O que o design fez:** passo 2 com número e largura do pé, recomendação que diz quando subir um número.
- **Não pode piorar:** custo de devolução de tênis usado (o teste de 30 dias permite correr com ele). Troca de tamanho e devolução com uso precisam ser contadas à parte.

### 3. Uso do configurador: acima de 45%
- **Fórmula:** sessões com `questionario_concluido` ou `modulo_trocado` antes de adicionar à sacola ÷ sessões que viram a PDP.
- **Olhar junto:** abandono por passo do questionário. Se a maioria sai no passo 1 (pisada), vale mudar a ordem, como já está anotado na reavaliação.
- **Não pode piorar:** tempo até adicionar à sacola. Configurar não pode virar obstáculo para quem já sabe o que quer.

### 4. Tíquete médio: +25%
- **Fórmula:** receita ÷ pedidos pagos. Junto: % de pedidos com acessório e % com segundo solado.
- **O que o design fez:** sugestões que mudam com o solado na sacola; segundo solado no desktop (no mobile, só depois do teste).
- **Não pode piorar:** conversão. Se o tíquete sobe e a conversão cai, a venda cruzada está atrapalhando.

## Como comparar
- **Linha de base:** 4 semanas do site atual, antes de trocar.
- **Teste A/B, 50% para cada versão**, se houver tráfego. Para ver a conversão sair de 1,8% para 3,2% com 95% de confiança e 80% de poder, são cerca de **2.000 sessões por versão**. Para uma melhora menor, até 2,5%, são cerca de **6.700 por versão**.
- **Devolução demora:** só dá para ler 30 dias depois da entrega. Para ver 22% virar 14%, são cerca de **360 pedidos por versão**.
- Sem tráfego para A/B, comparar antes e depois, sabendo que o calendário de provas mexe nas vendas de tênis de corrida.

## Impacto estimado (cenário, não previsão)
Com os números do brief: tíquete médio de R$ 1.800 (meio da faixa de R$ 1.400 a R$ 2.200), a cada 10.000 sessões.

| Cenário | Conversão | Pedidos | Receita | Devoluções por tamanho |
|---|---|---|---|---|
| Hoje (brief) | 1,8% | 180 | R$ 324.000 | ~40 (22%) |
| Metade do caminho | 2,5% | 250 | R$ 450.000 | ~35 (14%) |
| Meta do brief | 3,2% | 320 | R$ 576.000 | ~19 (6%) |

O cenário do meio é o que eu usaria numa conversa com o time: é o que se pode defender antes de ter dados. A meta do brief depende de tudo dar certo ao mesmo tempo. O tíquete médio maior (+25%) não entrou na tabela, para não somar duas apostas.
