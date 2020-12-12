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



*HEAD:* Estado atual do nosso código, ou seja, onde o Git nos colocou
*Working tree:* Local onde os arquivos realmente estão sendo armazenados e editados
*index:* Local onde o Git armazena o que será commitado, ou seja, o local entre a working tree e o repositório Git em si.

- [Filtros git log](https://devhints.io/git-log)
- [Fundamentos do Git](https://git-scm.com/book/pt-br/v2/Fundamentos-de-Git-Gravando-Altera%C3%A7%C3%B5es-em-Seu-Reposit%C3%B3rio)