# KINETIC // LAB — Escopo (Etapa 0)

Prazo: entrega em 16/11/2026. Projeto 3 do portfólio.

## Regra de honestidade
Pesquisa, entrevistas, personas e números são **simulados** (fictícios), por causa do prazo de 1 dia.
No estudo de caso, isso aparece escrito: "pesquisa simulada / proto-personas". Nunca apresentar como dado real.

## O que entra (MVP)
1. **Questionário de ajuste** ("Encontre seu ajuste") — 5 passos: pisada, peso, km/semana, terreno, foco. Resultado: entressola, drop e tamanho recomendados.
2. **PDP com troca de módulos** — vista explodida do tênis (cabedal / entressola / solado), troca por chips, preço atualiza na hora. 3D é simulado com camadas no Figma.
3. **Frete por CEP e custo por km** na PDP.
4. **Carrinho lateral (drawer)** com frete antecipado e cross-sell ligado ao módulo escolhido.
5. **Checkout em tela única** — Pix, cartão tokenizado, Apple/Google Pay, endereço de cobrança = entrega com 1 toque, selo de 30 dias.
6. Home e Catálogo com filtros (terreno, pisada, km, compatibilidade).

Mobile primeiro (390 px), depois desktop (1440 px) para Home, PDP e Checkout.

## Fica para a V2
Escaneamento do pé por câmera (AR), integração Strava/Garmin com aviso de troca de refil.

## Decisões sobre o brief
- "Biometric Fit & Stride Matcher" vira **"Encontre seu ajuste"** na interface (não há biometria, é questionário).
- Texto do brief em PT-PT ("face a", "num clique") → interface em PT-BR.
- Números do brief (68% abandono, 1,8%→3,2%) entram como **dados do brief / metas**, não como resultado.

## Produto e preços (definidos para o projeto)
Modelo: **KINETIC M1**. Base = cabedal + entressola + solado.

| Módulo | Opções | Preço |
|---|---|---|
| Base M1 (Aero Knit + Flow + Road Grip) | — | R$ 1.599 |
| Cabedal | Aero Knit (malha) · Ripstop (+R$ 120) · Storm, membrana impermeável (+R$ 240) | |
| Entressola | Flow (macia, drop 8 mm) · Pulse (placa de propulsão, drop 6 mm) · Stable (estabilidade p/ pronada, drop 10 mm) · Ground (drop 4 mm) | Pulse +R$ 200, demais inclusas |
| Solado | Road Grip (asfalto molhado) · Trail Lug (cravos 5 mm, terra/lama) | inclusos |
| Refil de entressola | dura ~600 km | R$ 349 |
| Solado avulso | | R$ 279 |
| Cross-sell | Meia anti-atrito R$ 89 · Palmilha de impacto R$ 189 · Sensor de cadência R$ 399 | |

Faixa de configuração: R$ 1.599 a R$ 2.039 (dentro do tíquete do brief, R$ 1.400–2.200).

**Conta do custo por km (corrigida):**
- KINETIC: base R$ 1.599 (1ª entressola) + 2 refis (R$ 698) = **R$ 2.297 para 1.800 km → R$ 1,28/km**
- Convencional: 3 pares de R$ 1.299 (600 km cada) = **R$ 3.897 para 1.800 km → R$ 2,17/km**
- Economia: **41%**. Frase na interface: "1 base KINETIC + 2 refis rodam 1.800 km por R$ 2.297. Três pares comuns custariam R$ 3.897."

## Cronograma de 1 dia
| Bloco | O quê |
|---|---|
| 1 | Escopo, CSD, benchmarking, personas, empatia, jornada (docs) |
| 2 | Sitemap, user flow, wireframes média fidelidade (Figma) |
| 3 | Design system + telas alta fidelidade mobile e desktop |
| 4 | Protótipo navegável + teste rápido (2 pessoas, se possível) |
| 5 | Estudo de caso + card no portfólio (com humanizer) |
