# git push

Veja em mais detalhes como utilizar o `git push` [aqui](https://git-scm.com/book/en/v2/Git-Branching-Remote-Branches).

## 🔥Usos comuns
- `git push <servidor> <branch>`-> envia o histórico de uma branch para o servidor remoto da url ou do nome configurado com o `git remote`
- `git push -f <servidor> <branch>`-> força o _push_ mesmo que sejam detectadas alterações no servidor remoto que não foram sincronizadas no repositório local

## ❌Erros comuns
### Foram detectadas modificações no repositório remoto que ainda não foram sincronizadas no repositório local 
![2022-03-02 (5)](https://user-images.githubusercontent.com/35473934/156451561-9fcee68d-2bf7-493a-b1a9-f347ff677d12.png)
#### ✔️Como solucionar: Sincronize o seu repositório local com o `git pull`


