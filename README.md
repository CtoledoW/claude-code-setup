# claude-code-setup

Plugin **oficial da Anthropic** para o Claude Code. Ele analisa o código de um projeto e recomenda as automações mais úteis para ele: servidores MCP, skills, hooks, subagentes e plugins.

> **Esta é uma cópia sem modificações**, mantida para fins educacionais. A fonte oficial e atualizada é o marketplace da Anthropic: [anthropics/claude-plugins-official › plugins/claude-code-setup](https://github.com/anthropics/claude-plugins-official/tree/main/plugins/claude-code-setup). **Recomendamos instalar sempre pela fonte oficial.**

## O que o plugin faz

O plugin contém a skill `claude-automation-recommender`. Ela:

1. lê o projeto (`package.json`, `pyproject.toml`, estrutura de pastas) para identificar linguagem, framework, banco de dados, testes e CI;
2. recomenda **uma ou duas** automações por categoria, ligadas ao que encontrou;
3. entrega um relatório dizendo onde cada recomendação seria configurada.

A skill é **somente leitura**: ela analisa e recomenda, mas não cria nem altera arquivos.

## Como instalar

### Pela fonte oficial (recomendado)

No Claude Code:

```text
/plugin install claude-code-setup@claude-plugins-official
```

Outra opção é procurar o plugin em `/plugin` › *Discover*.

### A partir deste repositório

```bash
git clone https://github.com/CtoledoW/claude-code-setup.git
claude --plugin-dir ./claude-code-setup
```

## Como usar

```text
Recomende automações do Claude Code para este projeto.
```

```text
Analise este repositório e me diga quais hooks eu deveria configurar.
```

## Créditos

- **Autoria:** Anthropic. A documentação original, em inglês, está em [`README.en.md`](README.en.md).
- **Repositório original:** [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official)
- **Alterações nesta cópia:** nenhuma no plugin. Foram adicionados este `README.md` em português, e o README original foi renomeado para `README.en.md`.

## Série *Do Planejamento ao Código*

Este repositório faz parte do material educacional gratuito *Do Planejamento ao Código — 5 Skills para Desenvolver Projetos com Inteligência Artificial*, da Brismarp Tecnologia.

| Capítulo | Repositório |
|---|---|
| 1. Planejamento e orquestração | [maestro](https://github.com/CtoledoW/maestro) |
| 2. Arquitetura e organização do ambiente | **claude-code-setup** (este) |
| 3. Desenvolvimento e implementação | [using-agent-skills](https://github.com/CtoledoW/using-agent-skills) |
| 4. Automação e produtividade | [convert-documents-to-markdown](https://github.com/CtoledoW/convert-documents-to-markdown) |
| 5. Qualidade e curadoria de ferramentas | [find-skills](https://github.com/CtoledoW/find-skills) |

## Licença

[Apache License 2.0](LICENSE), conforme o repositório original da Anthropic.

---

**Brismarp Tecnologia** — Inovação que conecta ideias ao futuro

Material gratuito e educacional. Se este repositório ajudou você, dê os créditos aos autores originais citados acima.
