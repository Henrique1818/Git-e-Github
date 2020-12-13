## Curso de Git e Github

#### Principais comandos

- git init -> Inicializar um repositório no diretório onde está o projeto na máquina local;

- git config --global user.name "nomeNome" -> adicionando um usuário global para o git;
- git config user.name -> Visualizar qual usuário está configurado;

- git config --global user.name "nome@dominio.com";

- git status -> Visualizar o estado dos arquivos no repositório;

- git add . -> adicionar todos os arquivos do projeto;

- git log -> visualizar os commits realizados, Hash é único para cada commit feito;
- git log --oneline -> visualizar os commits realizados em uma única linha;
- git log -p -> visualizar os commits e o que foi alterado nos commits;
- git log --pretty="format:%H" -> comando que nos traz apenas o hash;
- git log --pretty="format:%h %s" -> por sua vez, traz o hash resumido seguido pela mensagem do commit

- git branch -M main;
- git branch -> visualizar as branchs que tem;
- git branch <nome da branch> -> criar uma nova branch;
- git checkout <nome da branch> -> entrar na branch criada;
- git checkout -b <nome da branch> -> criar uma nova branch e ja está dentro dela;

- arquivo .gitignore -> ignorar os arquivos ou diretórios, escritos nele; 

- git init --bare -> compartilha um diretorio para ser como remoto;
- git remote add <nome> <url> -> adicionado um repositorio remoto;
- git remote rm <nome> -> remove o repositorio;
- git remote rename <nome> -> renomea o repositorio;
- git remote -v -> visualizar quais repositorios remotos existem;
- git clone <url> -> clona o um repositorio remoto;
- git push -u <nome> <branch> -> envia(empurrar) os commits para o repositorio;
- git push -> envia(empurrar) os commits para o repositorio;
- git pull <nome> <branch> -> puxar todos os dados do repositorio remoto da branch;
- git pull -> puxar todos os dados do repositorio;

- git pull origin main --rebase -> puxar as atualizações feitas na branch remota; 

- git merge <branch> -> juntar a branch de atualizações na master (:x para sair do terminal);

- git checkout -- index.html -> vai desfazer a modificação, (sem add ou commitar o arquivo);
- git reset HEAD index.html -> desfazendo modificação adicionada;
- git revert <nº do commit> -> desfazendo commit ja feito;

- git stash -> criando um armazenamento temporario, onde guarda informações que quero alterar depois;
- git stash list -> mostrar a lista de stash criadas;
- git stash drop -> apagar o stash criado;
- git stash apply 0 -> aplicar o stash criando no arquivo;
- git stash pop -> tirar e remove a stash e aplicar no arquivo;

- git checkout af0caaa -> voltando para o commit ja feito;
- git diff -> mostrar a diferença entre os commits;
- git diff <nº do commit.. > -> mostrar a diferença entre os commits (.. = ate);

- git log -n 2 -> mostrar os 2 ultimos commits;

- git tag -> mostar todas as tag criadas;
- git tag -a v0.1.0 -m "Lançando a primeira versão (BETA) da aplicação de cursos" -> criando uma tag no git;


*HEAD:* Estado atual do nosso código, ou seja, onde o Git nos colocou
*Working tree:* Local onde os arquivos realmente estão sendo armazenados e editados
*index:* Local onde o Git armazena o que será commitado, ou seja, o local entre a working tree e o repositório Git em si.

- [Filtros git log](https://devhints.io/git-log)
- [Fundamentos do Git](https://git-scm.com/book/pt-br/v2/Fundamentos-de-Git-Gravando-Altera%C3%A7%C3%B5es-em-Seu-Reposit%C3%B3rio)
- [Rebase e merge](https://medium.com/datadriveninvestor/git-rebase-vs-merge-cc5199edd77c)