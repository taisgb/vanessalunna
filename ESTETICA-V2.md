# estetica-v2

Referência visual: Clínica Estética Vanessa Lunna. Snapshot da versão atual da main em 27/11/2026, preservado na branch estetica-v2. A main continua dedicada à cliente.

## Identidade
Estética premium editorial, sem números decorativos, sem contadores, sem setas decorativas, sem textos genéricos nem repetição de fotos. Cormorant Garamond e Manrope. Paleta original nude, creme, taupe, marsala e champagne; adaptar à marca de cada lead, inclusive os gradientes SVG e cores específicas no CSS.

## Elementos que devem ser preservados
- Navbar fixa, flutuante, pill, glass, com blur e menu mobile.
- Hero com fundo integral desde o topo, retrato original à direita, foco no rosto e cabelo, integração por máscara, texto à esquerda, botões pill e arcos discretos.
- Faixa SVG inline, nunca imagem rasterizada. Preservar geometria atual (extremidade esquerda mais baixa, centro elevado, direita elevada), espessura, alinhamento da trilha textPath, sobreposição e animação contínua. As regras finais de .hero + .ribbon definem a posição responsiva. Não alterar isoladamente o path ou o margin-top; testar a junção em todas as larguras.
- Cards fotográficos com alinhamento e profundidade; biografia assimétrica; tratamentos em lista editorial; seção regenerativa escura.
- Texturas procedurais SVG e gradientes orgânicos nas redes sociais e localização. Na seção social, início e fim do gradiente em var(--cream), integrando seções adjacentes.
- Instagram incorporado com link alternativo e YouTube; Google Maps incorporado e botão Traçar rota; FAQ, rodapé e contato flutuante.
- Reveal por IntersectionObserver, transforms, hover e suporte a prefers-reduced-motion. Sem scroll lateral.

## Adaptação para cada cliente
Copiar a estrutura de index.html, assets/style.css e assets/main.js. Substituir nome, marca, fotografias, procedimentos, formação, registro profissional, links de contato, redes sociais, mapa, metadados e favicon. Não reutilizar fotos, contatos ou dados de Vanessa em outras prévias. Usar somente materiais adequados e autorizados, evitar depoimentos e resultados inventados. O iframe de Instagram depende de permissão de incorporação; manter alternativa por link. Manter noindex durante prospecção, lembrando que não é controle de acesso. Versionar CSS após mudanças; revisar desktop/mobile, enquadramento, faixa, links, contraste e performance antes de publicar. Esta branch é uma referência de código, não um gerador parametrizado; a conferência visual final das últimas mudanças permanece pendente.

## Arquitetura
HTML estático, CSS e JS vanilla, WebP, SVG inline, integrações externas carregadas sob demanda. Não requer framework ou build.
