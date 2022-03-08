# git reset

Permite navegar entre commits em uma _branch_. Entender esse comando lhe permitirá retornar para pontos antigos do projeto e desfazer commits. Mais detalhes [aqui](https://git-scm.com/book/pt-br/v2/Git-Tools-Reset-Demystified).

## 🔥Usos comuns
- `git reset --soft <commit>`-> move o ponteiro HEAD para o commit especificado sem alterar os arquivos na área de trabalho.
- `git branch --mixed <nome>`-> além de executar o que o _soft_ faz, remove os arquivos da _staging area_ retornando para o ponto antes de executar `git add`.
- 🚨`git branch --hard <nome>`-> restaura as modificações da área de trabalho. <b>Esse comando deve ser utilizado com precaução, já que modificações não commitadas não poderão ser recuperadas</b>. 

## Comandos relacionados
### [git commit](https://github.com/viniirbr/github-tutorial/blob/main/Comandos%20Essenciais/git-commit.md)
Registra o estado atual de um conjunto de arquivos no repositório.

