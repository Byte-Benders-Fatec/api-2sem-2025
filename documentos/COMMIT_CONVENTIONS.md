## :bookmark_tabs: Padrão de Commits

Nosso projeto segue o padrão **[Conventional Commits](https://www.conventionalcommits.org/pt-br/v1.0.0/)** adaptado com **emojis** para facilitar a identificação do tipo de mudança.

| Emoji | Código | Tipo      | Descrição                                                                 | Exemplo de uso                                      |
|-------|------|-----------|---------------------------------------------------------------------------|-----------------------------------------------------|
| ✨     | `:sparkles:` | **feat**   | Nova funcionalidade adicionada                                            | `✨ feat(auth): adicionar login com Google`          |
| 🐛     | `:bug:` | **fix**    | Correção de bug                                                          | `🐛 fix(api): corrigir erro 500 ao criar usuário`    |
| 📚     | `:books:` | **docs**   | Alterações na documentação                                                | `📚 docs(readme): adicionar instruções de instalação`|
| 🎨     | `:art:` | **style**  | Mudanças de formatação/estilo (sem impacto no código)                    | `🎨 style: padronizar indentação com Prettier`       |
| ♻️     | `:recycle:` | **refactor** | Refatoração de código sem alteração de comportamento                    | `♻️ refactor(user-service): extrair validações`      |
| ⚡     | `:zap:` | **perf**   | Melhorias de performance                                                  | `⚡ perf(query): otimizar busca por índice`          |
| ✅     | `:white_check_mark:` | **test**   | Adição ou modificação de testes                                           | `✅ test(auth): adicionar teste de refresh token`    |
| 🛠️     | `:hammer_and_wrench:` | **build**  | Mudanças em build, dependências ou ferramentas                           | `🛠️ build:  atualizar express para ^4.19.0`           |
| 🤖     | `:robot:` | **ci**     | Alterações em configuração de CI/CD                                       | `🤖 ci: adicionar workflow de testes no GitHub`      |
| 🚚     | `:truck:` | **chore**  | Tarefas diversas sem impacto no código funcional (scripts, limpeza, etc.) | `🚚  chore: remover arquivos temporários`             |
| ⏪     | `:rewind:` | **revert** | Reversão de commit anterior                                               | `⏪ revert: "feat(auth): adicionar refresh token"`   |
| 🚀     | `:rocket:` | **release**| Marcação de versão/release                                                | `🚀 release: v1.0.0`                                |

---

### Modelo de commit

```
[Emoji opcional] <tipo>[escopo opcional]: <descrição>

[corpo opcional]

[rodapé(s) opcional(is)]
```

---

### Exemplo de commit (com `corpo` e `rodapé`)
```bash
git commit -m ":sparkles: feat(auth): adicionar refresh token (#123)" \
 -m "Implementa rota POST /auth/refresh e guarda jti no Redis para revogação." \
 -m "Refs: #123"
```

---

> **Regras gerais:**
> - Mensagem curta no **imperativo** (ex.: “adicionar”, “corrigir”).
> - Usar escopo quando aplicável: `tipo(escopo): descrição`.   
> - Opcional: corpo do commit para explicar “porquê” da mudança.
> - Opcional: rodapé do commit para informações extras:  
>    - Referências a issues/PRs (`Refs: #123`).  
>    - Alterações que quebram compatibilidade (`BREAKING CHANGE:`).

---
