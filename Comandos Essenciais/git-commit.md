# git commit

Um dos conceitos fundamentais do _Git_, o _commit_ é uma 'fotografia' dos estados de um conjunto de arquivos. Esse registro é comumente feito quando uma funcionalidade é implementada ou correção é feita. Para saber melhor quando fazer o commit, confira [essa resposta no Stack Overflow](https://pt.stackoverflow.com/questions/17503/qual-a-quantidade-apropriada-de-altera%C3%A7%C3%B5es-para-um-commit). O _commit_ também deve vir acompanhado de uma mensagem, descrevendo qual alteração foi realizada. Uma boa descrição de como escrever essa mensagem está [nesse artigo](https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/).

<b>Informações mais detalhadas em: </b> [Gravando Alterações em Seu Repositório](https://github.com/viniirbr/github-tutorial/tree/main/Comandos%20Essenciais).

## 🔥Usos comuns
- `git commit -m <mensagem>`-> cria um commit com a mensagem de descrição.
- `git commit -a -m <mensagem>`-> manda todos os arquivos que sofreram modificação para a 'área de commit' (_stagin area_) e cria um commit com a mensagem de descrição.

## Comandos relacionados
### [git reset](https://github.com/viniirbr/github-tutorial/blob/main/Comandos%20Essenciais/git-reset.md)
Desfaz commits
### git add
Adiciona arquivos modificados ou adicionados no projeto à _staging area_.
