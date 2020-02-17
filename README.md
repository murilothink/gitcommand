# Curso de Git CI&T

git diff (mostra a alteração)
git ckeckout <nome do arquivo> (volta o estado atual da banch)
git reset --hard  (apaga tudo que está no status ou exclui o arquivo)

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

### git tag

marcar commit especifico, para poder voltar a uma tag especifica.

git tag v1.0.0 origin/master
git push --tags

### git fetch 

Faz downloads de todas a Branch cridas para saber as alterações

git fetch origin
git fetch --all

  
