# AGENTS.md — Instruções Canônicas para Agentes

Este arquivo é a fonte principal de instruções compartilhada por todos os agentes deste repositório. Preserve e siga as instruções específicas do projeto.

<!-- shared-agent-pr-policy:v1 -->
## Política Compartilhada de Branches, Revisão e Pull Requests

- Aplica-se a Hermes, Codex, OpenCode, Antigravity e demais agentes; preserve as regras específicas de segurança, privacidade, permissões e custo do projeto.
- Para tarefas que alteram arquivos, trabalhe em branch própria da tarefa, nunca diretamente na branch padrão. Abra um PR por objetivo e atualize o PR existente ao continuar o mesmo trabalho.
- Antes de abrir ou atualizar PR, atualize a referência da branch base e revise o diff completo contra ela, procurando regressões, mudanças fora do escopo e segredos. Rode `git diff --check` e as verificações/testes relevantes; corrija os problemas encontrados e registre bloqueios reais.
- Se houver no Orca outro agente gratuito disponível, solicite uma segunda revisão do diff em modo somente leitura. Não use fallback pago. Registre no PR se a revisão ocorreu, qual agente/modelo e o resultado, ou a indisponibilidade/motivo. Não declare revisão/testes que não foram executados.
- O PR deve incluir resumo, verificações e resultados reais, estado da segunda revisão e pendências. O merge e o auto-merge são exclusivos do usuário; agentes não devem executar nenhum dos dois.
- Preserve alterações locais preexistentes. Use worktree isolado por repositório; para repositórios ainda não disponíveis no Orca, use clone separado.
<!-- /shared-agent-pr-policy:v1 -->
