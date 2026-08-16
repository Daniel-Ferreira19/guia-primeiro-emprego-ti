# Aprendizados

## Sobre o processo de versionamento

Este projeto foi minha primeira experiência criando e gerenciando um repositório Git do início ao fim, incluindo branches separadas por finalidade, pull requests, e a resolução de um conflito de merge real.

## O que aprendi na prática

- A diferença entre `git fetch`, `git reset` e `git revert` ficou muito mais clara depois de precisar usá-los para corrigir um erro real: mergear uma branch diretamente pelo terminal antes de abrir o Pull Request correspondente. Usar `git reset --hard` para desfazer essa mudança local, sem afetar o histórico remoto, me ajudou a entender na prática quando cada comando é apropriado.
- Entendi por que um merge fast-forward não gera um commit de merge separado, e por que isso importa ao decidir entre `reset` e `revert`.
- Provocar um conflito de merge de propósito ajudou a entender que o Git não decide sozinho qual versão de uma mudança deve prevalecer — ele apenas identifica a divergência e devolve a decisão para quem está integrando o código.

## Dificuldades encontradas

No início, tive dificuldade em diferenciar comandos de sistema de arquivos (como `mkdir` e `New-Item`) dos comandos Git, além de confundir a ordem correta do fluxo (branch → commit → push → pull request → merge). Repetir esse fluxo em cada módulo do guia ajudou a fixar a sequência.

## Conclusão

Além do aprendizado técnico sobre Git e GitHub, este projeto me fez refletir sobre o próprio tema do guia que escrevi — a dificuldade de ingressar na área de TI —, já que produzir este material em paralelo à minha própria preparação para um processo seletivo tornou a reflexão mais concreta e pessoal.