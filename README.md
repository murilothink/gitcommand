# Curso de Git CI&T

![Murilo](https://i.imgur.com/XLn2CAt.png)



![Murilo](https://i.imgur.com/lvDLMoH.png)

git diff (mostra a alteração)
.

git ckeckout <nome do arquivo> (volta o estado atual da banch)
  
  
git reset --hard  (apaga tudo que está no status ou exclui o arquivo)

### Listar Commit

git log --pretty=oneline (Você controla completamente o que o log mostra. Eu gosto do formato de linha única)

git log

### Git Log 

git log --pretty=oneline --max-count=2

git log --pretty=oneline --since='5 minutes ago'

git log --pretty=oneline --until='5 minutes ago'

git log --pretty=oneline --author=<your name>
  
git log --pretty=oneline --all

git log --all --pretty=format:"%h %cd %s (%an)" --since='7 days ago' ( Apenas as modificações que eu fiz ) 

git log --pretty=format:"%h %ad | %s%d [%an]" --graph --date=short ( Apenas as modificações que eu fiz [formato adequado])

### Criar Branch 

git branch 


git branch feature/jira-333 (criação da branch)

### Git Checkout

Git checkut master


git checkout -b feature/jira-333


git  checkout index.html

### Git Stash

Salvar o estado da Branch e voltar para o estado inicial

git stash


git stash list


git stash pop


git stash apply

### Git  rebase -i

Deixar sua Branch direrente com o da master, manter organizado

git rebase -i origin/develop


git rebase -i origin/master


git rebase -1 HEAD~3 (AGRUPANDO COMMIT)

### git tag

marcar commit especifico, para poder voltar a uma tag especifica.

git tag v1.0.0 origin/master


git push --tags

### git fetch 

Faz downloads de todas a Branch cridas para saber as alterações

git fetch origin
git fetch --all (ver as breach novas )

### Git Pull

Vai atualizar sua Branch e vai enserir na sua master 

git pull
git fetch + git merge

### Git Push
Envia seus commit e objetos de uma branch 

git psuh origin master

## git diff   

mostram as alterações que foram feitas

git diff 

### 
 teste repositorio

Execute o comando git cherry-pick {hash} para trazer um commit para a branch master. Substitua {hash} pelo hash que foi copiado no passo 6;

Confira que apenas a alteração desejada foi aplicada no master, e não toda a branch novo-release;

Execute o comando git rebase novo-release e confira que o Git executa apenas um trabalho, embora hajam dois commits na nova branch, pois um já foi trazido para o master;

Altere o título da página (na tag <title>) para "Lista de cursos de DevOps";

Execute git add index.html e git commit -m "Adicionando DevOps no título" para commitar esta alteração;

Altere o título da página (na tag <title>) para "Lista de cursos da Alura";

Execute git add index.html e git commit -m "Mudando título" para commitar esta alteração;

Altere o título da página (na tag <title>) para "Cursos da Alura";

Execute git add index.html e git commit -m "Mexendo no título" para commitar esta alteração;

Altere o título do arquivo (na tag <title>) para "Lista de cursos";

Execute git add index.html e git commit -m "Título alterado" para commitar esta alteração;

Execute o comando git bisect start para informar ao Git que você vai iniciar uma busca por determinada alteração;

Execute o comando git bisect bad HEAD para informar que o estado atual do código está "ruim", ou seja, o título não está no estado que você quer;

Executando git log --oneline, copie o hash do commit com a mensagem "Simplificando o título";

Execute o comando git bisect good {hash}, substituindo {hash} pelo hash copiado no passo anterior, para informar que o estado atual do código está "bom", ou seja, o título está no estado que você quer;

Confira no código que agora o título está como você quer;

Execute git bisect good para informar ao Git que neste commit o código ainda está como você quer;

Confira no código que agora o título não está mais como você quer;

Execute git bisect bad para informar ao Git que neste commit o código não está mais como você quer;

Note que o Git encontrou o exato commit onde o título deixou de estar no estado em que você quer;

Execute git bisect reset para indicar que você finalizou a busca;

Execute o comando git show {hash}, substituindo {hash} pelo hash conferido no passo 30. Veja que é exatamente a alteração que você estava buscando;


. 

Para reverter esta alteração, execute git revert {hash}, substituindo {hash} pelo hash conferido no passo 30. Resolva quaisquer conflitos que possam ter sido encontrados;

Execute git blame index.html e confira o responsável por cada linha do arquivo.

teste4
