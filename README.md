## Startup settings
git config --global user.name <..> - name for making commit 
git config --global user.email <..> - email address
git config --list  

## Main commands
git init - initialize new repo
git status - show commit status (show list files which ready to commit), show current repo status
git add <files> - add files which need to save in repo (add changes to index), make files ready for commit
git commit -m "<message>"- make commit (save in repo)  
git log - history of changes  
git checkout <commit hash>- go to commit hash version
git checkout <branch name> - go to "branch name" branch
git cat-file -t <hash> - read hash file
git cat-file -p <hash> - cat commit information
git checkout master - back to 'master' branch (back pointer HEAD)  

## Trackable status
untracked
Unmodified
Modified
Staged

## Objects type in GIT

Blob - file  
Tree - folder
Commit 
Annotated Tag  
Commit - pointer to tree 
Branch - link to last commit  

## Branches in GIT

git branch <branch name> - creating branch 
git checkput <branch name> - change to branch (pointer HEAD to 'branche name')  
git checkout -b <branch name> - creating branch and to it  
git branch - current branches list
git branch -m <new branch name> - rename current branch
git branch -d <branch name> - delete branch

## Cлияние веток

git merge <feature branch name> - слияние другой ветки feature branch name в текущую receiving branch  
создание ветки new-feature  
перейти в new-feature  
внести изменение в проект  
сделать коммит в new-feature  
перейти обратно в main и также создать коммит  
выполнить слияние new-feature в main  
после слияния удалить new-feature  

## GitHub. Основы работы
git clone <url> - скачать удаленный репозиторий себе на комп  
origin - имя удаленного репозитория по умолчанию  
git branch -a - отображать все ветки, включая ветки с удаленного репозитория  
git pull - загрузка и применение изменений с удаленного репозитория в локальный  
git push - загрузка изменений из локальной ветки в ветку удаленного репозитория  
git remote add origin <url> - подключение удаленного репозитория  
git push -u origin <branch> - загрузка в удаленный  
git pull - скачать  
git branch -vv  

## Дополнительные команды GIT
##############################################################################
git rebase - перемещение коммитов с одной ветки в другую  
git rebase onto - указывается коммит. с которого начинается перебазирование(отложенные изменения)  
git stash push  
git stash pop - вернуть отложенные изменения с очищением папки где хранились  
git stash apply - вернуть отложенные изменения без очищением папки где хранились  
git stash list  
git stash show - показать отложенные изменения  
git stash drop - удалить отложенные изменения  
git stash clear - очистить хранилище  
git remote - спислк названий удаленных репозиторий  
git fetch - подтягивает изменения с удаленного репозитория  
git pull - скачивание позитория  
git clone [url] - слонирование репозитория себе на ПК локально 
git remote rm <name> - удаление удаленного репозитория  
