# git rebase

Tem o mesmo objetivo de mesclagem, porém realiza a tarefa de forma a manter o histórico mais limpo, como se não tivesse ramificações. Informações detalhadas de como utilizar [aqui](https://git-scm.com/book/pt-br/v2/Branches-no-Git-Rebase).

## 🔥Usos comuns
- `git rebase <branch>`-> mescla _branch_ à branch atual.

## ⚙️Como funciona
  <p align='center'>  <img src='https://git-scm.com/book/en/v2/images/basic-rebase-1.png' width='400px'></p>
  
  ```
  git checkout experiment
  git rebase master
  ```
  
  O Git parte do ancestral comum das branches e vai registrando em arquivos temporários as diferenças entre os commits. Em seguida, redefine a branch para a branch desejada e refaz os commits um a um. No exemplo acima, a differença do commit C4 é salvo em um arquivo temporário, alteramos para a branch master e o commit é recriado como C4'.
  
   <p align='center'>  <img src='https://git-scm.com/book/en/v2/images/basic-rebase-3.png' width='400px'></p>

  

## Comandos relacionados
### [git checkout](https://github.com/viniirbr/github-tutorial/blob/main/Comandos%20Essenciais/git-checkout.md)
Para alterar a branch em que o usuário está navegando utilize o comando `git checkout <branch>`
### [git merge](https://github.com/viniirbr/github-tutorial/blob/main/Comandos%20Essenciais/git-merge.md)
Para trazer os commits de uma branch para outra faça um checkout para a branch que irá receber os commits e dê um `git merge <branch>`, onde 'branch' é de onde os commits virão
### [git branch](https://github.com/viniirbr/github-tutorial/blob/main/Comandos%20Essenciais/git-branch.md)
Manipula as branches do repositório, seja criando, renomeando, deletando, entre outros.
