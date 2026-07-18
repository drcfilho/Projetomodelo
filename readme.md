# README.md

# Estrutura Padrão do Repositório

Este repositório segue uma metodologia baseada em Agile, Scrum, Desenvolvimento Modular, Documentação Contínua e Arquitetura Orientada à Evolução.

## Documentos do projeto

- README.md — guia do repositório.
- prompt.md — base obrigatória para a criação de qualquer prompt.
- plan.md — documento mestre do projeto.
- architecture.md — arquitetura técnica, módulos, APIs, banco, integrações e padrões.
- design.md — UI/UX, design system, layout, tipografia, bibliotecas CSS e componentes.
- sprints.md — planejamento das Sprints.
- tasks.md — backlog operacional da Sprint.
- pendencias.md — bugs, dívidas técnicas e melhorias futuras.
- decisions.md — registro das decisões arquitetônicas (ADR).
- git.md — fluxo e padronização do Git.

> **Nota sobre o Projeto Modelo (Placeholders):** 
> Alguns arquivos deste repositório modelo (como `README.md`, `plan.md`, `sprints.md`, `architecture.md`, `design.md` e `tasks.md`) podem estar inicialmente vazios. Eles servem como um lembrete estrutural de que precisam ser criados e preenchidos sob demanda durante o ciclo de vida do projeto, utilizando os agentes e o arquivo `prompt.md` como base.

## Diretório de Agentes (`agents/`)

A pasta `agents/` armazena os prompts de sistema e as regras de atuação para cada especialista (agente) envolvido no projeto.
- Contém os arquivos de persona para cada especialista (ex: `product-owner.md`, `scrum-master.md`, `software-architect.md`, `frontend.md`, `backend.md`, etc.).
- Contém o arquivo `agent-rules.md`, que consolida as regras globais (como a Verificação Prévia Obrigatória) e o foco específico de cada papel.
- Cada agente deve ser inicializado com as instruções contidas em seu respectivo arquivo dentro desta pasta, garantindo que atuem sempre de acordo com o fluxo e a metodologia do repositório.

## Diretório de Documentação (`docs/`)

A pasta `docs/` armazena 03 arquivos `manual.md` que vai conter o manual do sistema completo. sera um dos ultimos arquivos a serem feitos, o `implantar.md` com o manual de tudo que tem de ser feito para implantar com um checklist e o `testlocal.md` ensinando como fazer o teste local e como zerar o bd para implantar.

## Diretrizes de Interação

- **Uso do `prompt.md`:** É estritamente obrigatório utilizar o arquivo `prompt.md` como modelo/base para qualquer prompt a ser criado ou enviado aos agentes neste projeto.

## Fluxo obrigatório

1. Ler plan.md
2. Consultar architecture.md
3. Consultar design.md
4. Planejar a Sprint
5. Executar uma única tarefa por vez
6. Executar os testes
7. Atualizar tasks.md
8. Registrar pendências
9. Atualizar architecture.md/design.md quando necessário
10. Registrar decisões em decisions.md
11. Executar o fluxo descrito em git.md

Toda documentação deve permanecer sincronizada com o código.
