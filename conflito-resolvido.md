# Conflito Resolvido

## O que causou o conflito

Foi provocado um conflito de merge de propósito, para fins de aprendizado. A mesma linha do arquivo `README.md` (seção "Autoria") foi editada de duas formas diferentes:

- Na branch `main`, o texto foi alterado para: `Daniel Ferreira V. de Araújo`
- Na branch `feature/conflito-teste` (chamada localmente de `teste`), o texto foi alterado para: `Daniel F. Vieira de Araújo`

## Como o conflito apareceu

Ao tentar integrar a branch `teste` na `main` com o comando `git merge teste`, o Git identificou que a mesma linha havia sido modificada de forma diferente nos dois lados, e não conseguiu decidir automaticamente qual versão manter. O merge foi interrompido com a mensagem:

## Como foi resolvido

O arquivo `README.md` foi aberto no editor, onde o Git marcou o trecho conflitante com os marcadores `<<<<<<<`, `=======` e `>>>>>>>`, mostrando as duas versões lado a lado. Após analisar as duas opções, o conflito foi resolvido manualmente, definindo o texto final da linha de autoria e removendo os marcadores.

Em seguida, o arquivo resolvido foi adicionado à staging area e commitado, finalizando o merge: