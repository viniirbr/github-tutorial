# git merge

Esse comando incorpora commits de outra branch para a branch atual. Para sabr mais, veja essa [página](https://git-scm.com/book/pt-br/v2/Branches-no-Git-O-b%C3%A1sico-de-Ramifica%C3%A7%C3%A3o-Branch-e-Mesclagem-Merge).

## 🔥Usos comuns
- `git merge <branch>`-> mescla os commits de _branch_ à branch atual.

## ⚙️Tipos de merge
  ### fast-foward
  ```
  git checkout master
  git merge hotflix
  ```
  
<p align='center'><img src='https://git-scm.com/book/en/v2/images/basic-branching-4.png' width='400px'></p>

   <b>A branch que sefrerá o _merge_ (hotflix) está diretamente à frente da branch atual (master), então o comando simlesmente move o ponteiro HEAD para o último commit de hotflix.</b>

<p align='center'><img src='https://git-scm.com/book/en/v2/images/basic-branching-5.png' width='400px'></p>

  
  ### estratégia recursiva
  ```
  git checkout master
  git merge iss53
  ```
  
<p align='center'><img src='https://git-scm.com/book/en/v2/images/basic-merging-1.png' width='400px'></p>

   <b>O Git percebe que o histórico divergiu em algum ponto mais antigo. Nesse caso, ele parte do ancestral comum aos dois e cria um novo _snapshot_(fotografia) incorporando 
  os commits da branch desejada. Perceba que esse novo commit terá dois pais, o que pode ser visualizado com o comando `git log --graph`</b>
<p align='center'><img src='https://git-scm.com/book/en/v2/images/basic-merging-2.png' width='400px'></p>
  
## 🚧Conflitos de merge
  
  Quando são detectadas modificações no mesmo local de um arquivo em duas branches que estão sendo mescladas, o processo é suspenso e retorna uma mensagem de _merge conflict_. O Git marca automaticamente no seu arquivo os locais de conflito com as duas informações conflitantes para que você possa decidir o que fazer. Ao realizar as alterações, apague as marcações, adicione à _staging area_ (`git add`) e faça o commit. Orientações mais detalhadas são dadas [aqui](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-using-the-command-line).

## Comandos relacionados
### [git checkout](https://github.com/viniirbr/github-tutorial/blob/main/Comandos%20Essenciais/git-checkout.md)
Para alterar a branch em que o usuário está navegando utilize o comando `git checkout <branch>`
### [git branch](https://github.com/viniirbr/github-tutorial/blob/main/Comandos%20Essenciais/git-branch.md)
Manipula as branches do repositório, seja criando, renomeando, deletando, entre outros.
### [git rebase](https://github.com/viniirbr/github-tutorial/blob/main/Comandos%20Essenciais/git-rebase.md)
Desempenha o mesmo papel do `git merge`, mas o git deleta os commits de uma branch e recria na outra de modo a 'esconder' a utilização de branches no histórico do projeto
