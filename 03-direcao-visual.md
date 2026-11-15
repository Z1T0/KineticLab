# KINETIC // LAB — Direção visual

## Referências e o que levar de cada uma

### 3. lumiê (base principal) — https://future-glaze-22299415.figma.site/
Loja de pulseiras com berloques, feita no Figma Make. Já resolve o configurador modular.
- **Configurador "Monte a sua"**: prévia ao vivo à esquerda, passos numerados à direita (01 Escolha sua pulseira, 02 Adicione berloques), total e botão de adicionar fixos embaixo. → vira o **configurador da PDP**: 01 Cabedal · 02 Entressola · 03 Solado, com prévia do tênis em vista explodida.
- Barra de aviso no topo (frete grátis) → "30 dias de teste na corrida · Frete grátis acima de R$ 1.500".
- Faixa em movimento (marquee) entre seções → "ROAD-TO-TRAIL ✦ 1.800 KM ✦ TROQUE SÓ O QUE GASTOU".
- Cards de produto com tag (Best-seller, Novo) e favorito, preço com "ou 10x sem juros".
- Seção escura editorial com foto de um lado e texto do outro.
- Bloco de manifesto em fundo colorido com uma palavra em destaque → "Troque só o que gastou."
- Faixa de 3 garantias com ícone antes do rodapé (Sua de verdade / Compra tranquila / Qualidade) → 30 dias de teste · Pagamento seguro · Peças trocáveis.
- Rodapé escuro com newsletter em linha e 3 colunas de links.
- O link do Figma (hwgRBE694Fbj7MKwaLU6gG, "E-commerce de Pulseiras e Tênis") é o mesmo projeto, incorporado do Figma Make; não há parte de tênis.
- Título com contraste de duas fontes (grotesca pesada + serifada itálica). → Na KINETIC, a segunda voz é **mono técnica** (dados de engenharia), não serifa.

### 1. Sports News
- Títulos enormes em caixa alta sobrepostos à foto do atleta recortado → hero com o tênis explodido em peças.
- Mosaico de categorias foto/texto → filtros por terreno no catálogo.
- Tags com borda e botões pretos com seta.

### 2. Sport Tênis
- Paleta preto + verde, hero escuro, faixa de benefícios abaixo do hero.
- Evitar: grid estreito, texto pequeno, verde claro sobre branco com contraste baixo.

## Design system proposto

### Cores
| Token | Hex | Uso |
|---|---|---|
| Ink | #0D0F0E | Texto principal, botões primários, fundos escuros |
| Asfalto | #1B1F1D | Superfícies escuras secundárias |
| Grafite | #5A605C | Texto secundário (AA sobre Paper) |
| Linha | #D9DCD3 | Bordas, divisores |
| Paper | #F3F4EF | Fundo da página |
| Branco | #FFFFFF | Cards |
| Verde Pista | #13753F | Preços, links, sucesso, seleção (AA sobre branco e Paper) |
| Sinal (lime) | #C8F23A | Destaque **só sobre fundo escuro** (badges, foco, marquee) |
| Erro | #B42318 | Erros de formulário |
| Alerta | #9A5B00 | Avisos (estoque baixo, prazo) |

### Tipografia
- **Archivo** (Black / ExtraBold, largura expandida) — títulos em caixa alta
- **Inter** — texto corrido, botões, formulários
- **JetBrains Mono** — dados técnicos (drop 6 mm, 600 km, R$ 1,28/km, SKU)

### Formas
- Raio: 4 (tags), 12 (inputs, chips), 20 (cards, painéis), 999 (botões pill, como na lumiê)
- Botão primário: pill preto com seta →; secundário: borda Ink
- Foco: anel de 2 px Sinal sobre escuro / Verde Pista sobre claro
- Alvo de toque mínimo de 48 px no mobile

### Tom
Engenharia de corrida, nada de "moda". Mais laboratório que vitrine: números visíveis, explicação do porquê de cada peça.
