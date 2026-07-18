# Fluxo de atualização do repositório (branch `master`)

Execute os comandos abaixo na ordem:

# Atualiza as referências do repositório remoto sem alterar os arquivos locais
git fetch origin

# Adiciona todas as alterações, incluindo arquivos novos, modificados e excluídos
git add -A

# IMPORTANTE:
# Antes de executar o commit, analise as alterações realizadas (por exemplo, com `git status`
# e `git diff --stat`) e escreva uma mensagem que descreva fielmente o que mudou.
# A mensagem do commit deve ser gerada com base nas alterações efetuadas,
# nunca uma mensagem genérica.

git commit -m "Mensagem descritiva baseada nas alterações realizadas"

# Atualiza a branch local com a versão mais recente da master
git pull --rebase origin master

# Envia as alterações para o GitHub
git push origin master
```

## Boas práticas

- Use mensagens de commit específicas e objetivas.
- A mensagem deve refletir exatamente as mudanças realizadas no projeto.
- Exemplos:
  - `git commit -m "Remove arquivos obsoletos e atualiza dependências"`
  - `git commit -m "Corrige validação do agendamento de RG"`
  - `git commit -m "Refatora autenticação e ajusta layout da tela inicial"`
