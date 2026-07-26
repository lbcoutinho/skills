# Instruções para agentes trabalhando neste repositório

Este repositório é uma lista curada pessoal de **skills, agentes, frameworks e ferramentas** para desenvolvimento de software com agentes de IA (Claude Code e afins), no estilo de [awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code).

Arquivos principais:
- `README.md` — lista principal, organizada por categoria.
- `REJECTED.md` — recursos já avaliados e descartados (com motivo).
- `templates/entry.md` — template e convenções de formatação de entrada.

## Fluxo de curadoria

Quando o usuário mandar um link de um repositório/ferramenta novo:

1. **Pesquise o recurso** (README do repo, descrição, exemplos) para entender o que ele faz.
2. **Escolha a seção** mais adequada no `README.md` (Skills, Agentes/Subagentes, Frameworks & SDKs, MCP Servers & Integrações, Ferramentas & CLIs, Observabilidade & Monitoramento, Segurança, Documentação & Aprendizado). Se nenhuma servir bem, crie uma nova seção (adicione também no índice).
3. **Adicione a entrada** seguindo o template de `templates/entry.md`, com a etiqueta `🧪 pending test`. Insira em ordem alfabética dentro da seção. Remova a linha `_Nenhuma entrada ainda._` se for a primeira entrada da seção.
4. Se o usuário não pedir para commitar/pushar, apenas edite os arquivos localmente e avise que a entrada foi adicionada — não faça commit automaticamente a menos que seja instruído ou que o fluxo de trabalho da sessão já preveja isso.

Quando o usuário disser que um recurso foi **testado e aprovado**:
- Troque a etiqueta `🧪 pending test` por `✅ approved` na entrada correspondente no `README.md`.
- Opcionalmente, enriqueça a descrição com uma nota de uso real.

Quando o usuário disser que um recurso foi **rejeitado**:
- Remova a entrada do `README.md`.
- Adicione ao `REJECTED.md` no formato do template, com a data e o motivo da rejeição (peça o motivo se o usuário não tiver dado um).

## Convenções gerais

- Entradas em ordem alfabética dentro de cada seção.
- Descrições objetivas e curtas (1–2 frases), sem tom de marketing.
- Nunca duplicar um recurso já presente em `README.md` ou `REJECTED.md` — se o link já existir em `REJECTED.md`, avise o usuário em vez de readicionar automaticamente.
- Para o fluxo guiado passo a passo, existe a skill `curate-resource` (`.claude/skills/curate-resource/SKILL.md`).
