# git branch

O conceito de _branching_ (ramificação) pode ser melhor compreendido [aqui](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell).

## 🔥Usos comuns
- `git branch`-> lista as branches existentes
- `git branch <nome>`-> cria uma branch
- `git branch -m <nome antigo> <novo nome>`  -> renomea uma branch 
- `git branch -d <nome>`-> deleta uma branch

## Comandos relacionados
### [git checkout](https://github.com/viniirbr/github-tutorial/blob/main/Comandos%20Essenciais/git-checkout.md)
Para alterar a branch em que o usuário está navegando utilize o comando `git checkout <branch>`
### [git merge](https://github.com/viniirbr/github-tutorial/blob/main/Comandos%20Essenciais/git-merge.md)
Para trazer os commits de uma branch para outra faça um checkout para a branch que irá receber os commits e dê um `git merge <branch>`, onde 'branch' é de onde os commits virão
### [git rebase](https://github.com/viniirbr/github-tutorial/blob/main/Comandos%20Essenciais/git-rebase.md)
Desempenha o mesmo papel do `git merge`, mas o git deleta os commits de uma branch e recria na outra de modo a 'esconder' a utilização de branches no histórico do projeto
