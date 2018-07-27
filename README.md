# Dicas para uso do git


* Fiz pull, deu conflito no merge e quero desfazer o pull (para excluir a branch local);
````
git merge --abort
````
* Remover branch local
````
git branch -D 'branch_name'
````
* Adicionar repositório remoto
````
git remote add upstream <url_do_repositorio_remoto>
````
* Criar branch local a partir da remota
````
git fetch upstream <branch_remota>:<branch_local>
````
* Baixar pull request para teste local
````
git fetch upstream pull/<id>/head:<branch_local>
git checkout <branch_local>
````
* Atualizar branch local com código do pull request
````
git pull upstream pull/<id>/head
````

