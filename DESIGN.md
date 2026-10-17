---
name: "cloudpet"
description: "Uma landing calorosa e monumental para a história de saúde conectada do pet."
colors:
  cloudpet-blue: "#2859c5"
  cloudpet-blue-dark: "#1847ad"
  ink: "#000000"
  paper: "#ffffff"
  lilac-snow: "#f4f6ff"
  lilac-mist: "#e7ebfe"
  muted-ink: "#4a4a4a"
  focus-gold: "#f0c852"
typography:
  display:
    fontFamily: '"ChunkFiveEx", "Chunk Five", Rockwell, Georgia, serif'
    fontSize: "clamp(76px, 12.3vw, 177px)"
    fontWeight: 400
    lineHeight: 0.765
    letterSpacing: "-0.035em"
  headline:
    fontFamily: '"ChunkFiveEx", "Chunk Five", Rockwell, Georgia, serif'
    fontSize: "clamp(58px, 5.85vw, 84px)"
    fontWeight: 400
    lineHeight: 0.92
    letterSpacing: "-0.02em"
  title:
    fontFamily: '"Livvic", Arial, sans-serif'
    fontSize: "28px"
    fontWeight: 700
    lineHeight: 1.2
  body:
    fontFamily: '"Livvic", Arial, sans-serif'
    fontSize: "18px"
    fontWeight: 500
    lineHeight: 1.45
  label:
    fontFamily: '"Livvic", Arial, sans-serif'
    fontSize: "15px"
    fontWeight: 700
    lineHeight: 1.45
rounded:
  menu: "16px"
  pet-card: "22px"
  compact-container: "28px"
  large-container: "56px"
  pill: "999px"
spacing:
  xs: "8px"
  sm: "16px"
  md: "24px"
  lg: "28px"
  xl: "40px"
  section-gap: "56px"
  inset: "72px"
  section: "140px"
components:
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.cloudpet-blue}"
    typography: "{typography.display}"
    rounded: "{rounded.pill}"
    padding: "10px 29px 15px"
    height: "62px"
  button-outline-hover:
    backgroundColor: "{colors.cloudpet-blue}"
    textColor: "{colors.paper}"
    typography: "{typography.display}"
    rounded: "{rounded.pill}"
    padding: "10px 29px 15px"
    height: "62px"
  button-light:
    backgroundColor: "{colors.lilac-snow}"
    textColor: "{colors.cloudpet-blue}"
    typography: "{typography.display}"
    rounded: "{rounded.pill}"
    padding: "13px 36px 18px"
    height: "72px"
  hero-chip:
    backgroundColor: "transparent"
    textColor: "{colors.lilac-snow}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "9px 23px 11px"
    height: "46px"
  service-detail:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    columns: "333px 645px"
    gap: "64px"
  belief-card:
    backgroundColor: "{colors.lilac-snow}"
    textColor: "{colors.ink}"
    rounded: "36px"
    border: "2px solid {colors.lilac-mist}"
    padding: "28px"
  section-panel:
    backgroundColor: "{colors.lilac-mist}"
    textColor: "{colors.ink}"
    rounded: "{rounded.large-container}"
    padding: "87px 72px 88px"
---

# Design System: cloudpet

## Overview

**Creative North Star: "A História Conectada"**

A identidade transforma prontuário e rotina de cuidado em uma experiência acolhedora, direta e memorável. O campo azul cloudpet funciona como mundo próprio; sobre ele, títulos slab monumentais, a matilha central e pequenos controles em cápsula equilibram expressão e utilidade.

O sistema é amigável sem parecer infantil. Superfícies lilás-neve, cantos amplos e ilustrações de produto dão leveza à informação de saúde, enquanto texto preto e navegação simples mantêm clareza. A composição alterna momentos de grande impacto com blocos calmos e muito espaço, sempre conduzindo tutor e clínica pela mesma história.

Este documento cobre a landing estática construída em `index.html`, `styles.css` e `script.js`. Ele registra sua linguagem visual e seus componentes presentes; não define a interface interna do aplicativo ou do dashboard.

**Key Characteristics:**

- Azul cloudpet como cenário, ação e elo entre as seções.
- Tipografia slab grande e compacta para mensagens de marca.
- Superfícies claras, bordas lilás e cantos generosos.
- Cápsulas leves para ações e metadados, nunca como decoração indiscriminada.
- Fotografia e mockups recortados que entram na composição, sem molduras genéricas de aplicativo.

## Colors

A paleta combina um azul confiante e saturado com neutros frios quase brancos; preto e cinza preservam legibilidade, enquanto dourado aparece somente como sinal de foco.

### Primary

- **Azul cloudpet:** ocupa hero e CTA, colore títulos funcionais, marcadores, links ativos e a ação contornada.
- **Azul cloudpet profundo:** reserva um tom de apoio mais escuro dentro da família principal; não substitui o azul dominante sem motivo funcional.

### Secondary

- **Tinta da carteirinha:** mantém a microtipografia do documento legível e coerente com sua superfície azul clara.
- **Marca da carteirinha:** desenha o detalhe de QR code sem competir com o conteúdo.

### Neutral

- **Tinta:** cor principal de texto e de títulos fora dos painéis azuis.
- **Papel:** fundo geral, menu móvel e inversão de texto sobre o azul.
- **Neve lilás:** texto sobre azul e preenchimento da ação clara.
- **Névoa lilás:** bordas, divisores e painel de etapas.
- **Tinta atenuada:** informação de baixa ênfase, como o copyright.
- **Dourado de foco:** contorno acessível para navegação por teclado.

### Named Rules

**The Blue Field Rule.** Use o azul cloudpet em grandes campos ou ações claras; não o fragmente em muitos acentos pequenos concorrentes.

**The Cold Neutral Rule.** Painéis de apoio permanecem na família lilás-neve, preservando contraste suave com o papel branco.

**The Focus Is Signal Rule.** O dourado existe para foco visível e não vira cor promocional.

## Typography

**Display Font:** ChunkFiveEx (com Chunk Five, Rockwell, Georgia e serif como fallback)  
**Body Font:** Livvic (com Arial e sans-serif como fallback)

**Character:** ChunkFiveEx dá voz robusta, arredondada e afetiva às mensagens principais; Livvic mantém navegação, explicações e metadados leves e legíveis. O contraste entre as famílias é deliberado e sustenta a personalidade inteira da landing.

### Hierarchy

- **Display** (400, fluido de 76px a 177px, 0.765): reservado ao título monumental do hero; no mobile, reduz para a faixa de 36px a 56px e relaxa levemente a entrelinha.
- **Headline** (400, fluido de 58px a 84px, 0.92): títulos de seção; a CTA amplia a mesma voz para 104px em desktop.
- **Title** (700, 28px, 1.2): títulos das etapas; detalhes de serviço usam ChunkFiveEx em 38px com numerais de 72px.
- **Body** (500, 18px, 1.45): leitura corrente; introduções e textos-chave sobem para 22px, enquanto descrições compactas usam 17px.
- **Label** (700, 15px, caixa alta): agrupadores e rótulos de navegação; links principais chegam a 26px no desktop.

### Named Rules

**The Slab Owns the Message Rule.** Chunk Five é usada em grandes promessas, nomes de recursos e numerais de processo; explicação e navegação permanecem em Livvic.

**The Tight Monument Rule.** Títulos slab grandes usam entrelinha compacta e tracking negativo; nunca ganham entrelinha de texto corrido.

## Layout

A página usa um shell central de até 1360px com respiro lateral de 40px por lado. O desktop alterna grids assimétricos: introdução 820px/380px, detalhes de serviço em 333px/645px com lados alternados, história em proporção 1/2 e crenças em três colunas, além da CTA com coluna visual de 541px. O dashboard encerra a sequência de serviços centralizado em até 991px. O ritmo de seção principal começa com 140px de espaço superior, e blocos expressivos recebem 56px ou 72px de inset.

Em até 1120px, o shell cai para margens laterais de 20px e os grids assimétricos passam a proporções flexíveis. Em até 900px, a navegação vira menu de toque e as crenças passam para duas colunas. Em até 760px, o shell usa 16px por lado; hero, detalhes de serviço, etapas, história, crenças e CTA entram em fluxo de uma coluna, imagens preservam sua proporção intrínseca, raios grandes caem de 56px para 28px e o espaçamento superior reduz. Em até 380px, atalhos do hero e links do rodapé também se empilham.

**The One Hero Center Rule.** O primeiro viewport centra título e matilha no mesmo eixo; notas laterais e atalhos podem orbitar esse eixo, mas não competir com ele.

**The Collapse, Don't Squeeze Rule.** Grids de conteúdo colapsam para uma coluna no mobile; mockups não são comprimidos em colunas estreitas.

## Elevation & Depth

O sistema é plano por padrão. Profundidade vem de campos tonais, recortes de imagem, sobreposição e escala; detalhes editoriais não usam caixas ou sombras. A única sombra estrutural está no menu móvel flutuante, onde comunica que a navegação está acima da página.

### Shadow Vocabulary

- **Menu móvel flutuante** (`0 14px 34px rgba(40, 89, 197, 0.14)`): usada somente no painel de navegação aberto abaixo do cabeçalho móvel.

### Named Rules

**The Tonal Depth Rule.** Separe superfícies com mudança de azul, branco e lilás antes de recorrer a sombra.

**The Shadow Has a Job Rule.** Sombra indica uma camada realmente flutuante; não é acabamento padrão de cards.

## Shapes

Grandes áreas de marca usam cantos amplos de 56px no desktop e 28px no mobile. Elementos menores variam entre 16px e 22px, e ações são cápsulas completas. Bordas são raras, claras e funcionais: 2px no menu, 3px na ação contornada e 1px no chip do hero. Os celulares levemente inclinados quebram organicamente a geometria alinhada.

**The Scale the Radius Rule.** Quanto maior a superfície, maior o raio; controles pequenos não herdam o mesmo arredondamento visual dos painéis.

## Components

### Buttons

- **Shape:** cápsula completa, com altura mínima de 62px no desktop.
- **Primary:** a landing usa uma ação clara sobre azul, com neve lilás, texto azul e Chunk Five em 34px.
- **Outlined:** fundo transparente, borda azul de 3px e texto azul; no hover, torna-se um campo azul com texto branco.
- **Hover / Focus:** sobe 2px em 180ms; foco visível recebe contorno dourado de 3px com offset de 4px.
- **Mobile:** a ação clara reduz para 58px de altura mínima e 28px de texto; a CTA do cabeçalho desaparece para ceder lugar ao menu.

### Chips

- **Style:** chip transparente sobre o hero, com borda de 1px na cor do texto, raio de cápsula e padding compacto.
- **Use:** identifica a dupla de produtos “APP & Dashboard”; não funciona como uma taxonomia repetitiva.

### Cards / Containers

- **Service detail:** composição editorial sem caixa; alterna mockups de celular de 333px e texto de até 645px com 64px de intervalo. Numeral azul, título slab e descrição Livvic formam a hierarquia.
- **Steps panel:** névoa lilás sem borda ou sombra, raio de 56px e inset generoso; numerais slab azuis organizam a sequência.
- **Blue panels:** hero e CTA usam azul cloudpet, texto claro, recorte de imagem e raio de 56px; no mobile adotam 28px.
- **Dashboard detail:** fecha a sequência de serviços com texto centralizado e mockup de notebook de até 991px; no mobile volta ao alinhamento de leitura à esquerda.
- **Belief card:** superfície neve lilás com borda névoa de 2px e raio de 36px; fotografia recortada lidera, seguida por título ChunkFiveEx azul e descrição curta em Livvic. No mobile, o raio cai para 28px e a arte ocupa uma faixa de 170px.

### Navigation

- **Desktop:** três links Livvic em caixa alta e peso 700, com 112px de distância; ativo, hover e foco revelam uma linha inferior de 3px em 220ms.
- **Mobile:** botão circular contornado de 46px transforma duas linhas em “X”; abre painel branco de 210px, borda lilás, raio de 16px e sombra azul ambiente.
- **Behavior:** clicar em qualquer link fecha o menu e restaura rótulo e estado ARIA.

### Reveal Motion

- **Hero title:** aparece em 780ms com recorte, leve blur e deslocamento vertical usando uma curva de desaceleração expressiva.
- **Hero pets:** entra em 900ms, com atraso de 90ms, blur leve, escala e deslocamento ascendente.
- **Apoios do hero:** cabeçalho, nota, chip e atalhos completam a abertura em uma sequência curta de 180ms a 440ms.
- **Serviços:** imagem e texto chegam de lados opostos em 700ms para materializar a ideia de informação conectada; no mobile, ambos sobem pelo mesmo eixo de leitura.
- **Crenças:** título e cards entram como um grupo, com stagger curto de 60ms entre itens e atraso total abaixo de 200ms.
- **Demais seções:** usam uma única revelação por viewport, com deslocamento de 30px, blur limitado e recorte vertical.
- **Acessibilidade:** `prefers-reduced-motion` remove deslocamento, blur e recorte; falha ou ausência de `IntersectionObserver` mantém todo o conteúdo visível.
- **Reduced motion:** desativa scroll suave e reduz animações e transições a 0.01ms quando o usuário solicita menos movimento.

## Do's and Don'ts

### Do:

- **Do** manter o azul cloudpet como grande gesto visual e os neutros frios como áreas de leitura.
- **Do** reservar Chunk Five para mensagens, títulos de recurso e numerais que precisam de personalidade.
- **Do** adaptar grids por colapso e reduzir raios e espaçamentos de forma coordenada no mobile.
- **Do** usar imagens recortadas como parte da composição e preservar seus textos alternativos úteis.
- **Do** manter foco dourado visível e suporte a `prefers-reduced-motion` em qualquer novo estado interativo.

### Don't:

- **Don't** introduzir sombras em cards estáticos; use borda e contraste tonal.
- **Don't** transformar o hero em um layout genérico de texto à esquerda e mockup à direita.
- **Don't** misturar uma terceira família tipográfica ou usar Livvic para imitar a voz slab.
- **Don't** inventar depoimentos, métricas, logos de clientes ou destinos de conversão que a landing não possui.
- **Don't** extrapolar estes padrões para telas internas do app ou dashboard sem examinar essas superfícies.
