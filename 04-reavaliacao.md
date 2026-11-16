# KINETIC // LAB · Reavaliação do projeto (15/11, véspera do teste)

> **Nota de 16/11:** o teste com pessoas reais citado abaixo não aconteceu. Na noite de 15/11 ele foi trocado por um percurso cognitivo com 5 perfis simulados por IA ([08-avaliacao-simulada.md](08-avaliacao-simulada.md)). O roteiro está pronto e o teste continua pendente. Também tirei deste arquivo as contagens da descoberta simulada e reescrevi a enquete sugerida no item 1.

Leitura do arquivo inteiro do Figma (páginas 00 a 11), feita como faria quem avalia um portfólio. Também rodei uma auditoria automática nas telas, olhando tamanho de texto, contraste, números inconsistentes e espaços reservados esquecidos.

## Veredito
O projeto está pronto para ser mostrado. O processo dá para seguir do brief à tela, e cada decisão tem um porquê escrito. O ponto fraco continua sendo a pesquisa: ela é simulada, e o teste de amanhã é a única evidência real. Por isso, o que mais pesa daqui para frente é **fazer o teste bem e mostrar o que mudou por causa dele**.

## O que está forte
1. **Processo rastreável.** As 12 páginas estão numeradas, cada tela tem nota de "por quê", e há um diário com datas.
2. **Leitura crítica do brief.** Cinco mudanças justificadas, incluindo a conta dos 41% que não fechava no enunciado.
3. **Honestidade.** O que é simulado está marcado (aviso na capa, "persona fictícia", "dados fictícios" na ficha técnica), e as ferramentas de IA estão creditadas.
4. **Revisão crítica antes do teste.** Ela achou duas falhas que impediam tarefas do teste, e a página 11 já mostra o antes e depois da PDP.
5. **Design system com estados.** Foco, erro, sucesso, esgotado e desabilitado, com contraste calculado. A auditoria não achou texto pequeno nem contraste ruim nas telas.
6. **Identidade própria.** A "Fig. 01", com a vista explodida anotada, e o hodômetro tiram o projeto do visual de template.

## Corrigido nesta revisão
- A página 01 ainda falava em "configurador biomecânico", o que contradizia a mudança nº 1 do brief (tirar a promessa de biometria). Agora diz "configurador simples, guiado por um questionário de 5 perguntas".
- O hodômetro dizia "começa a contar no primeiro treino", mas no MVP não há integração com Strava ou relógio, então o site não teria como contar. Agora é um **hodômetro estimado**, calculado pelo volume que a pessoa informou no questionário. A contagem automática ficou marcada como V2.

## Riscos e o que eu faria (em ordem de impacto)

### 1. A pesquisa é toda simulada (alto)
Quem avaliar vai perguntar sobre isso.
- **Hoje, se der tempo:** mande 3 perguntas para 5 a 10 corredores (grupo de corrida, WhatsApp):
  1. "Você já desistiu de comprar tênis online por medo de errar o tamanho?"
  2. "Sabe qual é a sua pisada?"
  3. "Da última vez que você comprou um tênis de corrida, quanto pagou e por quanto tempo usou?"
- A terceira pergunta era "Pagaria R$ 1.599 num tênis que dura o triplo trocando só a espuma?". Ela embutia o benefício na pergunta, "o triplo" nem é o que a conta mostra, e intenção de compra declarada não prevê compra. A nova pergunta registra o que a pessoa já fez, e a conta do custo por km fica para o produto mostrar.
- Mesmo poucas respostas reais valem mais que as citações simuladas e podem confirmar ou derrubar a CSD.

### 2. O questionário começa pela pergunta mais difícil (médio)
A primeira pergunta é sobre a pisada, e a matriz CSD tem como dúvida justamente se o corredor sabe dizer a própria pisada.
- **Não mude antes do teste.** Observe se as pessoas travam ou usam o "Não sei".
- Se travarem, isso vira um achado da Iteração 1: começar por tamanho e terreno, que são fáceis, e deixar a pisada para o fim.

### 3. As metas não têm plano de medição (médio)
As metas do brief estão na página 01 (conversão de 1,8% para 3,2%, devolução de 22% para menos de 6%), mas não há como saber se o design atingiu cada uma.
- Um quadro curto de eventos resolve e mostra pensamento de produto: questionário concluído, tamanho recomendado aceito, módulo trocado, acessório adicionado, etapa do checkout, devolução por tamanho.

### 4. Limites do protótipo que podem enviesar o teste (médio)
- Os chips Ripstop, Storm, Flow, Pulse e Ground não respondem ao toque.
- O checkout mostra sempre 2 itens.
- A tarefa 2 pede a "sola de trilha", mas o chip se chama "Trail Lug", em inglês, com "terra e lama" embaixo. Isso testa se o nome é entendido, o que é bom, mas anote se alguém hesitar ali.

### 5. Tamanho: a maior dor tem a solução mais leve (médio)
O brief atribui 68% do abandono à dúvida de tamanho (dado do cliente, ainda a verificar), mas a recomendação se apoia no "número que você costuma usar". A opção "me ajude a medir o pé com uma folha A4" existe, mas não tem tela.
- Para o case, cite como próximo passo, ou desenhe uma tela simples de medição se sobrar tempo depois do teste.

### 6. Pequenas inconsistências (baixo)
- A tabela de produtos não mostra o preço do cabedal avulso. Por isso, o Storm a R$ 489 no catálogo parece não bater com o "+R$ 240" do configurador. A conta fecha (cabedal base de R$ 249 + 240), só não está escrita.
- A imagem do cabedal Storm mostra um tênis com outra sola.
- A logo usa uma fonte itálica e as telas usam Archivo Black reta. Não chega a conflitar, mas vale citar como decisão: a logo é a assinatura e a tipografia das telas privilegia a leitura.

### 7. Falta o estudo de caso escrito (alto, mas é o próximo passo)
O Figma mostra o processo, mas o recrutador lê o case primeiro. O case deve:
- abrir pelo problema e pelo resultado do teste, não pela lista de etapas;
- terminar com uma seção de **limites**, como nos projetos anteriores.

## Prioridade sugerida
1. **Hoje:** testar o protótipo no celular. Se der, mandar as 3 perguntas aos corredores.
2. **Amanhã de manhã:** fazer o teste com as 2 pessoas e anotar.
3. **Depois do teste:** preencher as páginas 10 e 11, montar o quadro de medição (item 3) e escrever o case.
