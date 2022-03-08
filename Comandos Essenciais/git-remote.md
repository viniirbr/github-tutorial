# git remote

Manipula o repositório remoto, local para onde as informações serão enviadas e de onde serão carregadas. Se o repositório é clonado do GitHub, o remoto padrão é chamado de _origin_. Caso seja inicializado localmente, é necessário criar o remoto com o comando `git remote add`. Saiba mais [aqui](https://git-scm.com/book/pt-br/v2/Fundamentos-de-Git-Trabalhando-de-Forma-Remota).

## 🔥Usos comuns
- `git remote`-> lista os repositórios remotos adicionados
- `git remote add <nome> <url>`-> adiciona o repositório remoto com _nome_ definido e associado a uma _url_.
- `git remote rename <nome antigo> <nome novo>`-> renomea um remoto 
- `git remote remove <nome>`-> remove um remoto
- `git remote get-url <nome>`-> retorna a url associada a um remoto

## Comandos relacionados
### [git pull](https://github.com/viniirbr/github-tutorial/blob/main/Comandos%20Essenciais/git-pull.md)
Atualiza o repositório local com as informações novas do servidor.
### [git push](https://github.com/viniirbr/github-tutorial/blob/main/Comandos%20Essenciais/git-push.md)
Atualiza o servidor com as informações novas do repositório.
