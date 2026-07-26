---
name: curate-resource
description: Adiciona, aprova ou rejeita um recurso (skill, agente, framework, ferramenta) na lista curada deste repositório. Use quando o usuário mandar um link de um repo/ferramenta novo para adicionar, disser que testou e aprovou um recurso já listado, ou disser que um recurso foi rejeitado/não presta.
---

# Curate Resource

Mantém `README.md` e `REJECTED.md` deste repositório atualizados seguindo o fluxo descrito em `CLAUDE.md`.

## Quando usar

- Usuário manda uma URL de repositório/ferramenta nova → **adicionar**.
- Usuário diz "testei o X e aprovei" / "pode marcar como aprovado" → **aprovar**.
- Usuário diz "o X não presta" / "rejeitei o X" / "remove o X" → **rejeitar**.

## Passo a passo

### 1. Adicionar novo recurso

1. Confira se o link já existe em `README.md` ou `REJECTED.md` (busque pela URL). Se já existir, avise o usuário em vez de duplicar.
2. Busque o conteúdo do link (WebFetch no README do repo, ou na página) para entender: o que faz, para que serve, autor/org.
3. Escolha a seção do `README.md` mais adequada (ver `CLAUDE.md` para a lista de seções). Crie uma nova seção só se nenhuma existente servir.
4. Insira a entrada em ordem alfabética na seção, seguindo `templates/entry.md`, com a etiqueta `🧪 \`pending test\``. Remova o placeholder `_Nenhuma entrada ainda._` se for a primeira entrada.
5. Confirme ao usuário em qual seção a entrada foi adicionada e com um resumo de 1 linha do que é o recurso.

### 2. Aprovar recurso existente

1. Localize a entrada no `README.md` (por nome ou link).
2. Troque `🧪 \`pending test\`` por `✅ \`approved\``.
3. Se o usuário der contexto de uso ("funcionou bem para X"), incorpore como uma nota curta na descrição.

### 3. Rejeitar recurso existente

1. Localize a entrada no `README.md`.
2. Remova-a do `README.md`.
3. Adicione ao `REJECTED.md`, no formato do template, com a data de hoje e o motivo. Se o usuário não deu motivo, pergunte antes de registrar (um motivo genérico não ajuda a decisão futura).

## Regras

- Nunca commitar/pushar automaticamente a não ser que o usuário peça ou o fluxo da sessão já exija isso — edite os arquivos e reporte o que mudou.
- Manter ordem alfabética dentro de cada seção.
- Descrições objetivas, sem marketing, 1–2 frases.
