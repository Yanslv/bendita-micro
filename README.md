# Projeto Bendita Micro — pacote para geração do site

Esta pasta reúne o material necessário para o Claude Code gerar o site Next.js da Bendita Micro / Ioná Victório.

## Arquivos principais

- `PRD.md`: requisitos completos do site e recomendação específica para a clínica.
- `site_config.json`: configuração inicial de marca, tema, seções, procedimentos e pendências.
- `PROMPT_CLAUDE_CODE.md`: prompt completo para colar no Claude Code.
- `research/analise_bendita_achados_parciais.txt`: evidências coletadas na análise do Instagram e do Bio Site.
- `assets/`: imagens de referência, manifesto de origem, inventário técnico e aviso de direitos de uso.

## Como usar no Claude Code

1. Abra o Claude Code dentro desta pasta.
2. Leia `PROMPT_CLAUDE_CODE.md` e cole o conteúdo no Claude Code, ou peça para ele ler o arquivo.
3. Execute a geração dentro de uma subpasta `site/`.
4. O código deve usar `site_config.json` como fonte inicial de conteúdo.
5. Antes de publicar, confirme endereço, WhatsApp, horários, formações, serviços, fotos, depoimentos e permissões de uso com a Ioná.

## Comando sugerido

```bash
claude
```

Depois, no Claude Code:

```text
Leia o arquivo PROMPT_CLAUDE_CODE.md e execute exatamente o plano. Antes de codificar, leia também PRD.md, site_config.json, research/analise_bendita_achados_parciais.txt e todos os arquivos de documentação em assets/. Gere o projeto Next.js em site/, rode lint, typecheck e build, corrija os erros e me entregue o resultado.
```

## Aviso sobre os assets

As imagens em `assets/` foram coletadas como referências públicas para análise e prototipação. Elas estão marcadas como `reference_only_pending_authorization` no manifesto. Não publique nenhuma imagem de cliente, resultado, logo ou material de marca sem autorização da profissional.
