# Prompt para Claude Code — Site Bendita Micro / Ioná Victório

Você é um engenheiro frontend sênior especializado em Next.js, TypeScript, UX mobile-first e páginas de conversão para profissionais de estética.

Quero que você gere um site em **Next.js com App Router, TypeScript e Tailwind CSS** para a marca **Bendita Micro / Ioná Victório**, com base nos arquivos deste diretório.

## 1. Antes de escrever código

Leia completamente estes arquivos antes de iniciar:

- `PRD.md`
- `site_config.json`
- `research/analise_bendita_achados_parciais.txt`
- `assets/README.md`
- `assets/manifest.csv`
- `assets/image_inventory.csv`

Use os arquivos como fonte de verdade para o posicionamento, estrutura, serviços e direção visual.

Não invente endereço, bairro, horários, preço, número direto de WhatsApp, credenciais, avaliações, depoimentos ou resultados clínicos.

Se algum dado estiver marcado como pendente, crie uma configuração editável e use um placeholder visual discreto ou o link público já confirmado. Não esconda pendências no código.

## 2. Objetivo do site

Criar uma landing page premium, pessoal e mobile-first para apresentar a Bendita Micro como especialista em:

- nanopigmentação personalizada de sobrancelhas;
- Nano Fios;
- micropigmentação labial;
- possível neutralização labial, que ainda precisa ser confirmada;
- design personalizado de sobrancelhas.

O objetivo principal é levar a visitante a tirar dúvidas e iniciar um agendamento pelo WhatsApp.

Mensagem central:

> Sobrancelhas e lábios pensados para valorizar a sua beleza.

CTA principal:

> Tirar dúvidas e agendar

CTA secundário:

> Conhecer os procedimentos

## 3. Direção visual

Crie uma estética feminina, sofisticada, acolhedora e especializada, sem parecer um template genérico de salão.

Use como ponto de partida a paleta sugerida em `site_config.json`:

- fundo: `#FAF6F3`;
- rosa suave: `#F0D9D8`;
- rosa queimado: `#B86F78`;
- vinho: `#7E3948`;
- texto escuro: `#2B2022`;
- dourado discreto: `#B59668`.

Use títulos com uma fonte elegante e textos com uma sans-serif legível. Evite excesso de fonte cursiva, excesso de sombras, gradientes fortes ou visual de clínica médica fria.

A experiência deve transmitir:

- técnica;
- cuidado;
- proximidade;
- precisão;
- feminilidade elegante;
- autoridade pessoal.

## 4. Imagens

Use somente imagens locais da pasta `assets/` durante o desenvolvimento.

Priorize os seguintes arquivos quando fizer sentido:

- `assets/asset_010_7a01c215ccc5d581.jpg` — retrato da Ioná em ambiente de atendimento;
- `assets/asset_011_b13b5a6a6ca17106.jpg` — close de lábios;
- `assets/asset_013_908c2b520eb77db1.jpg` — Ioná e ambiente de atendimento;
- `assets/asset_014_40f1b6f072c38c57.jpg` — referência visual de precisão e marca “by Ioná Victório”.

Antes de usar qualquer imagem, confira o `assets/manifest.csv`. Todas as imagens estão marcadas como `reference_only_pending_authorization`.

Como este é um protótipo comercial, exiba uma faixa ou selo discreto no topo informando:

> Demonstração visual — imagens e conteúdos dependem de validação e autorização antes da publicação.

Não use a marca do fornecedor “Concept Premium Blade” como se fosse uma certificação da Bendita Micro. A imagem `asset_014` pode ser usada apenas como referência visual, ou em uma seção sobre precisão/material, com cuidado.

Use `next/image` com `alt` descritivo. Não faça hotlink para URLs do Instagram.

## 5. Estrutura obrigatória da página

Implemente uma única página `/` com as seções abaixo:

### 5.1 Header

- logo textual “Bendita Micro”;
- assinatura “por Ioná Victório”;
- navegação por âncoras;
- botão “Agendar”;
- menu mobile funcional.

Como ainda não existe um arquivo de logo oficial, não desenhe um logo definitivo. Use uma marca tipográfica elegante e deixe o componente preparado para receber logo PNG/SVG depois.

### 5.2 Hero

Use o retrato da Ioná ou uma composição com retrato e close de procedimento.

Conteúdo sugerido:

- eyebrow: `Nanopigmentação personalizada em Cuiabá`;
- título: `Sobrancelhas e lábios pensados para valorizar a sua beleza.`;
- descrição: `Conheça os procedimentos da Bendita Micro e tire suas dúvidas com a Ioná antes de agendar.`;
- CTA principal para WhatsApp;
- CTA secundário para a seção de procedimentos.

O hero deve ficar excelente no celular e apresentar CTA sem exigir muita rolagem.

### 5.3 Autoridade

Criar uma seção curta com:

- Ioná Victório;
- especialista em nanopigmentação personalizada de sobrancelhas;
- foco em sobrancelhas e lábios;
- Cuiabá, somente como localização geral confirmada pelo perfil.

Não inventar formação específica. Criar uma área de especialização preparada para receber certificados posteriormente.

### 5.4 Procedimento principal — Nano Fios

Criar uma seção visualmente forte para Nano Fios/nanopigmentação de sobrancelhas.

Texto provisório:

> Uma técnica personalizada para valorizar o desenho e a expressão das sobrancelhas, respeitando as características de cada pessoa.

Adicionar CTA contextualizado:

> Quero entender o Nano Fios

### 5.5 Procedimentos

Criar cards para:

1. Nano Fios / Nanopigmentação de sobrancelhas;
2. Micropigmentação labial;
3. Neutralização labial — mostrar como “a confirmar” ou deixar configurável, pois o PRD indica que a nomenclatura precisa ser validada;
4. Design personalizado de sobrancelhas.

Cada card deve ter:

- imagem;
- título;
- descrição curta;
- botão de WhatsApp com mensagem específica;
- foco visual no procedimento principal.

### 5.6 Como funciona

Criar três ou quatro passos:

1. Você chama pelo WhatsApp.
2. A Ioná entende seu objetivo.
3. Você recebe as orientações.
4. O atendimento é agendado.

Deixar claro que a avaliação profissional orienta o procedimento. O site não faz diagnóstico.

### 5.7 Resultados e cicatrização

Criar uma galeria elegante e responsiva, mas com aviso de que os conteúdos dependem de autorização.

Não criar depoimentos falsos nem dizer que as imagens são “antes e depois” se isso não estiver confirmado.

Usar labels como:

- `Resultado visual de referência`;
- `Cicatrização — confirmar contexto`;
- `Imagem sujeita à autorização`.

### 5.8 Especialização

Criar seção para formação e especialização com estado pendente:

> A formação e as especializações da Ioná serão apresentadas aqui após validação dos certificados e informações oficiais.

A seção deve ficar pronta para receber:

- nome da formação;
- instituição;
- ano;
- certificado;
- descrição curta.

### 5.9 Sobre Ioná

Criar uma seção pessoal, usando retrato e texto provisório:

> Eu sou Ioná Victório, especialista em nanopigmentação personalizada de sobrancelhas e apaixonada por realçar a beleza de cada pessoa com técnica e cuidado.

Adicionar comentário no código/configuração indicando que o texto deve ser validado pela profissional antes da publicação.

### 5.10 Localização e contato

Como o endereço completo e os horários não foram confirmados, mostrar:

- `Cuiabá`;
- aviso “Endereço e horários serão confirmados pela profissional”;
- Instagram;
- CTA para WhatsApp.

Não inventar mapa, bairro ou horário.

### 5.11 FAQ

Implementar accordion acessível com estas perguntas:

- Como funciona a avaliação?
- Qual a diferença entre Nano Fios e design personalizado?
- Como funciona a micropigmentação labial?
- Como é o período de cicatrização?
- Quais cuidados são necessários?
- Onde fica o Studio Bendita Micro?
- Como faço para agendar?

As respostas devem ser marcadas como provisórias quando exigirem informação técnica da profissional.

### 5.12 CTA final

Título:

> Quer saber qual procedimento faz mais sentido para você?

Texto:

> Fale com a Ioná pelo WhatsApp e tire suas dúvidas antes de agendar.

Usar o link público confirmado no `site_config.json`:

`https://api.whatsapp.com/message/FBEWS5N5NRM3J1?autoload=1&app_absent=0`

Deixar o código preparado para substituir esse link por um número direto do WhatsApp Business depois.

### 5.13 Footer

Incluir:

- Bendita Micro;
- Ioná Victório;
- Instagram;
- Cuiabá;
- aviso de demonstração;
- link para WhatsApp;
- ano atual.

## 6. Implementação técnica

Use:

- Next.js com App Router;
- TypeScript;
- Tailwind CSS;
- componentes reutilizáveis;
- `next/image`;
- metadata e Open Graph;
- HTML semântico;
- acessibilidade de teclado;
- responsividade mobile-first;
- `lucide-react` ou ícones simples, se necessário;
- nenhuma dependência desnecessária.

Estruture o conteúdo em um arquivo de configuração tipado, por exemplo:

`src/config/site.ts`

Não espalhe textos e links por vários componentes. Os componentes devem consumir a configuração.

Componentes sugeridos:

- `Header`;
- `DemoNotice`;
- `Hero`;
- `AuthoritySection`;
- `ProcedureCard`;
- `ProcedureGrid`;
- `HowItWorks`;
- `ResultsGallery`;
- `SpecializationSection`;
- `AboutSection`;
- `LocationSection`;
- `FaqAccordion`;
- `WhatsappCta`;
- `Footer`.

## 7. WhatsApp

Centralize o link e as mensagens em configuração.

Mensagens:

- geral: `Olá! Vi o site da Bendita Micro e gostaria de saber mais sobre os procedimentos e o agendamento.`
- Nano Fios: `Olá! Vi as informações sobre Nano Fios e gostaria de entender como funciona a avaliação.`
- labial: `Olá! Gostaria de saber mais sobre micropigmentação labial e como funciona a avaliação.`
- design: `Olá! Gostaria de saber mais sobre design personalizado de sobrancelhas.`

Se o link público não permitir mensagem pré-preenchida, mantenha o CTA funcionando e deixe um comentário claro no código para substituir pelo número direto.

## 8. Segurança e conteúdo

- Não coletar dados clínicos.
- Não criar formulário solicitando informações sensíveis.
- Não inventar preço, endereço, credencial, avaliação ou resultado.
- Não afirmar que imagens públicas estão autorizadas.
- Não publicar depoimentos falsos.
- Não fazer promessas como “resultado garantido”, “sem risco” ou “definitivo”.
- Não usar imagens remotas do Instagram.
- Não fazer scraping.

## 9. SEO e metadata

Criar metadata em português:

- title: `Bendita Micro | Nanopigmentação de Sobrancelhas e Lábios em Cuiabá`;
- description: `Conheça os procedimentos da Bendita Micro com Ioná Victório e tire suas dúvidas sobre Nano Fios, sobrancelhas e micropigmentação labial.`;
- Open Graph com imagem local aprovada para demonstração;
- canonical configurável;
- favicon provisório tipográfico, sem afirmar que é o logo oficial.

## 10. Interações

Implemente:

- menu mobile abrir/fechar;
- scroll suave para âncoras;
- accordion da FAQ;
- hover/focus states;
- CTA flutuante de WhatsApp no mobile;
- galeria com `loading="lazy"` abaixo da primeira dobra;
- animações suaves e respeitando `prefers-reduced-motion`.

## 11. Qualidade

Depois de implementar:

1. rode lint;
2. rode typecheck;
3. rode build de produção;
4. corrija erros;
5. verifique todas as rotas e links;
6. confirme que todas as imagens locais carregam;
7. confirme que não existem placeholders acidentais como `undefined`, `null`, `Lorem ipsum` ou URLs quebradas;
8. confirme que o site não exibe dados não confirmados como fatos;
9. verifique a experiência em largura mobile e desktop;
10. entregue um resumo do que foi implementado e das pendências da clínica.

## 12. Entrega esperada

Gere o site funcional dentro deste diretório, preferencialmente em uma pasta `site/` para manter separados o briefing, os assets e o código.

Crie também:

- `site/README.md` com comandos para instalar, desenvolver e fazer build;
- `site/CONTENT_REVIEW.md` com os itens que Ioná precisa aprovar;
- `site/src/config/site.ts` com todos os textos e links centralizados;
- `site/public/assets/` com cópias somente dos assets usados no protótipo;
- uma lista dos assets usados e suas origens.

Não finalize apenas com explicações. Crie os arquivos, rode os testes e deixe o projeto executável.
