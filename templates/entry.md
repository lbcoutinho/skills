# Template de Entrada

Copie o bloco abaixo para a seção correta do `README.md`, substituindo os campos entre `< >`.

```markdown
- **[<Nome do Recurso>](<url-do-repo-ou-site>)** by [<Autor/Org>](<url-do-autor>) — 🧪 `pending test`
  <Descrição curta em 1–2 frases: o que faz, por que é interessante, o que o diferencia.>
```

Depois de testado, atualize a etiqueta de status:

```markdown
- **[<Nome do Recurso>](<url>)** by [<Autor>](<url-autor>) — ✅ `approved`
  <Descrição, agora podendo incluir uma nota curta de "por que aprovado" / como usar.>
```

Se o recurso for rejeitado, **remova** a entrada do `README.md` e adicione ao `REJECTED.md` neste formato:

```markdown
- **[<Nome do Recurso>](<url>)** — rejeitado em <YYYY-MM-DD>
  Motivo: <motivo objetivo da rejeição>.
```

## Convenções

- Ordenar entradas alfabeticamente dentro de cada seção.
- Descrição objetiva, sem marketing — o que o recurso faz de fato.
- Se o recurso servir mais de uma categoria, colocar na mais específica e, se fizer muito sentido, referenciar (link relativo) nas outras.
- Categoria não existe ainda? Criar uma nova seção no `README.md` (e no índice) em vez de forçar em uma existente.
