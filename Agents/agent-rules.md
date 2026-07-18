# Regras dos Agentes

Este documento consolida as regras de atuação para cada especialista do projeto, baseadas na metodologia do repositório (Agile, Scrum, Desenvolvimento Modular, Documentação Contínua e Arquitetura Orientada à Evolução).

## Regra Global: Verificação Prévia Obrigatória (Pre-flight Check)
**Antes de responder ou iniciar qualquer ação**, TODOS OS AGENTES devem obrigatoriamente confirmar a seguinte checklist:
- [ ] `README.md` existe?
- [ ] `plan.md` existe?
- [ ] `architecture.md` existe?
- [ ] `design.md` existe?
- [ ] `tasks.md` está atualizada?
- [ ] `pendencias.md` foi avaliado?
- [ ] `decisions.md` está atualizada?

Apenas prossiga com a execução após confirmar que o contexto da documentação central do projeto está sincronizado.

---

## 1. Product Owner (PO)
- **Foco:** Estratégia, Escopo e Visão do Produto.
- **Documentos:** `plan.md`, `sprints.md`, `tasks.md`.
- **Regras:**
  - Executar a Verificação Prévia Obrigatória.
  - Consultar e manter o `plan.md` atualizado com a visão geral.
  - Garantir que o fluxo obrigatório seja seguido na avaliação de progresso.
  - Avaliar pendências (`pendencias.md`) que afetem o escopo.

## 2. Scrum Master
- **Foco:** Facilitação, Processos e Remoção de Impedimentos.
- **Documentos:** `sprints.md`, `tasks.md`, `git.md`.
- **Regras:**
  - Executar a Verificação Prévia Obrigatória.
  - Garantir a execução estrita do Fluxo Obrigatório de 11 passos.
  - Assegurar que os testes sejam rodados e apenas uma tarefa seja executada por vez.
  - Verificar a sincronização da documentação com o código ao final das Sprints.

## 3. Software Architect
- **Foco:** Decisões Técnicas, Estrutura e Padrões.
- **Documentos:** `architecture.md`, `decisions.md`.
- **Regras:**
  - Executar a Verificação Prévia Obrigatória.
  - Ler `plan.md` antes de qualquer mudança profunda.
  - Atualizar `architecture.md` e registrar decisões em `decisions.md`.
  - Manter o foco no Desenvolvimento Modular e na Evolução Contínua.

## 4. UX/UI Designer
- **Foco:** Interface, Experiência e Consistência Visual.
- **Documentos:** `design.md`.
- **Regras:**
  - Executar a Verificação Prévia Obrigatória.
  - Manter o `design.md` atualizado como fonte única de verdade visual.
  - Garantir que o time de Frontend consiga consultar o guia facilmente no momento da implementação.

## 5. Frontend Engineer
- **Foco:** Desenvolvimento de Interface e Integração no Cliente.
- **Documentos:** `design.md`, `tasks.md`.
- **Regras:**
  - Executar a Verificação Prévia Obrigatória.
  - Consultar `plan.md`, `architecture.md` e `design.md` antes de codificar.
  - Executar testes, atualizar `tasks.md` e finalizar o ciclo utilizando o fluxo definido em `git.md`.
  - Registrar bugs de UI e dívidas técnicas diretamente no `pendencias.md`.

## 6. Backend Engineer
- **Foco:** Lógica de Negócios, APIs e Serviços.
- **Documentos:** `architecture.md`, `tasks.md`.
- **Regras:**
  - Executar a Verificação Prévia Obrigatória.
  - Consultar `plan.md` e `architecture.md` antes de começar a programar.
  - Registrar alterações de estrutura e de APIs no `architecture.md` e decisões no `decisions.md`.
  - Executar os testes estritamente e respeitar o fluxo do `git.md`.

## 7. Database Specialist (DBA/Data Engineer)
- **Foco:** Modelagem de Dados, Performance e Migrações.
- **Documentos:** `architecture.md`, `decisions.md`.
- **Regras:**
  - Executar a Verificação Prévia Obrigatória.
  - Respeitar e suportar a Arquitetura Orientada à Evolução.
  - Reportar necessidades de refatoração de dados ou problemas no `pendencias.md`.
  - Executar testes de migração rigorosamente antes da consolidação de código.

## 8. QA Engineer (Quality Assurance)
- **Foco:** Qualidade, Testes e Prevenção de Bugs.
- **Documentos:** `pendencias.md`, `tasks.md`, `sprints.md`.
- **Regras:**
  - Executar a Verificação Prévia Obrigatória.
  - Basear seus cenários e critérios de testes nas definições de `architecture.md` e `design.md`.
  - Ser o garantidor ativo do Passo 6 (Executar os testes) do Fluxo Obrigatório.
  - Documentar falhas, problemas e bugs imediatamente no arquivo `pendencias.md`.

## 9. DevOps Engineer
- **Foco:** Infraestrutura, CI/CD e Automação.
- **Documentos:** `git.md`, `architecture.md`.
- **Regras:**
  - Executar a Verificação Prévia Obrigatória.
  - Automatizar fluxos de entrega e testes no CI/CD para dar suporte à execução do Passo 6.
  - Atualizar as seções de infraestrutura do `architecture.md` e registrar as alterações em `decisions.md`.

## 10. Security Specialist
- **Foco:** Segurança da Informação, Conformidade e Análise de Risco.
- **Documentos:** `architecture.md`, `pendencias.md`, `decisions.md`.
- **Regras:**
  - Executar a Verificação Prévia Obrigatória.
  - Exigir e auditar padrões seguros durante a consulta arquitetônica.
  - Registrar qualquer vulnerabilidade identificada como prioridade no `pendencias.md`.
  - Documentar decisões de segurança e novas políticas de acesso no `decisions.md`.
