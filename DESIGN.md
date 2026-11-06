---
name: Echo Hub
version: "4.2"
colors:
  primary: "#3BFDE7"
  primary_strong: "#14D8C0"
  ink: "#0A0A0A"
  background: "#F8F9FA"
  surface: "#FFFFFF"
typography:
  display: "Bricolage Grotesque"
  body: "Inter"
  mono: "JetBrains Mono"
---

# Direção visual

O fundo claro é a base. Seções em preto dão contraste; o turquesa aparece como acento, luz e chamada para ação. Use superfícies lisas e bastante espaço. Evite manchas de luz flutuantes e excesso de efeitos.

## Cores

| Papel | Valor | Uso |
| --- | --- | --- |
| Turquesa | `#3BFDE7` | Acento, botão, foco e detalhes |
| Turquesa forte | `#14D8C0` | Hover, traços e contraste sobre claro |
| Turquesa para texto pequeno | `#0A6B60` | Rótulos sobre fundo claro |
| Preto da marca | `#0A0A0A` | Títulos, texto e seções escuras |
| Fundo claro | `#F8F9FA` | Base da página |
| Cartão | `#FFFFFF` | Superfícies elevadas |
| Cinza de apoio | `#6B7280` | Texto secundário sobre claro |
| Borda | `#E5E7EB` | Divisões discretas |

No fundo turquesa, use texto preto. Não substitua o preto da marca por `#000`.

## Tipografia

- **Títulos:** Bricolage Grotesque, peso 700–800, espaçamento entre letras de −.04em a −.05em.
- **Corpo e interface:** Inter, 16–18 px, entrelinha de 1.5–1.6.
- **Dados técnicos:** JetBrains Mono, apenas quando a leitura monoespaçada tiver utilidade.
- **Arquivos:** carregue `fonts.css` e os WOFF2 em `fonts/` (Bricolage Grotesque, Inter, Inter Outline 650 e JetBrains Mono); mantenha fallback de sistema.
- **Lettering vazado:** Inter 650, em trechos grandes do título. Desenhe o contorno antes do preenchimento com `paint-order: stroke fill`; o preenchimento deve ter a cor exata da superfície. Isso evita linhas internas atravessando as letras.

## Layout e componentes

- Contêiner de conteúdo até 1120 px, com margem lateral mínima de 16 px no celular.
- Botões e cartões pequenos usam raio de aproximadamente 12 px; cartões grandes, até 20 px.
- Botão principal sólido, com texto Inter semibold e altura de aproximadamente 48 px. Botões secundários têm contorno limpo. Origin UI orienta a base visual.
- ButtonCraft Neo Raised é uma exceção tátil para ações pontuais em superfícies claras. Evite aplicá-lo a todos os CTAs.
- Phosphor **Regular** é a família principal de ícones, em 20–24 px. Iconoir é apoio quando comunicar melhor uma ação. Não misture as duas famílias no mesmo componente.
- Para “Meta”, use `ph-crosshair` ou `iconoir-one-point-circle`. Não use `iconoir-target`.

## Marca e movimento

- `assets/logo-echo.png` sobre superfícies claras; `assets/logo-echo-branco.png` sobre superfícies escuras.
- `assets/echo-symbol.png` é o símbolo oficial para favicon e usos reduzidos; não o redesenhe com ícones de biblioteca.
- Prefira transições de 100–300 ms em interações. Momentos autorais maiores devem ter propósito e respeitar `prefers-reduced-motion`.
- No celular, reorganize blocos e controles para a largura disponível, sem rolagem horizontal. Priorize legibilidade e uma ação clara por bloco.

Veja `design-system.html` para a prévia visual, `tokens.css` para os valores CSS e `assets/` para os arquivos oficiais da marca.
