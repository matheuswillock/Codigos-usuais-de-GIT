# c-digo-usual

Códigos usuais

git pull
* Para ter certeza que temos o projeto 100% atualizada na master
git checkout -b nome-da-branch-nova
* Para criar a branch nova. Não pode haver espaço entre o nome da branch, mas deve conter o hífen
git clone 
* Para clonar o repositório.
git branch -D nome-da-branch 
* Para deletar uma branch criada.
git checkout master
*Para irmos para a Master.
git checkout nome-da-branch
*Para irmos para a branch desejável. Por exemplo: git checkout master — Para irmos para a Master.
Git add .
* Para adicionar as alterações para a branch especifica de nossa preferência, antes de subir um novo commit para a master.
git commit -m ‘nome_do_commit’
*usamos esse comando para commitar uma atualização nova para a master.
git push origin nome_da_branch
* Para abrir um pull request no github.
git merge nome_da_branch
* para ‘mergear’ o pull request do github
git push origin master
* Vai subir as atualizações para a Master.





CRIANDO CHAVE SSH


1. Acessar conta do https://github.com/

2. Rodar esse comando no terminal gitBash:
ssh-keygen -t rsa -b 4096 -C "programadorjedi@outlook.com"
ssh-keygen -t rsa -b 4096 -C "matheuswillock@outlook.com"

3. Apertar enter, enter, enter...

4. Rodar esse comando no terminal:

eval $(ssh-agent -s)

5. Rodar esse comando no terminal:

ssh-add ~/.ssh/id_rsa

6. Rodar esse comando no terminal:

WINDOWS:
clip < ~/.ssh/id_rsa.pub

MAC:
pbcopy < ~/.ssh/id_rsa.pub

LINUX:
xclip -sel clip < ~/.ssh/id_rsa.pub



Ele vai copiar a nossa chave assim que pressionarmos Control + V, a chave é colada.

7. Colar o código copiado pelo comando clip no github.com (em Configurações, Chaves SSH) > https://github.com/settings/keys


Dica: crie um nome específico fácil de reconhecer qual a máquina que está conectada com essa chave

Obs.: seria possível usar uma mesma chave em diferentes máquinas, mas aconselho usarem uma por máquina, pois se precisarem tirar o acesso de uma máquina, fica mais fácil de controlar.
