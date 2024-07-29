// configurando uma chave ssh
git version
git config --global user.name "Maria"
git config --global user.email "mariaeduardabenevenutti77@gmail.com"
git config --list
ls -al ~/.ssh
ssh.keygen -t ed25519 -C "mariaeduardabenevenutti77@gmail.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
clip < ~/.ssh/id_ed25519.pub

ssh -T git@github.com

// comando git - github
ls
cd Documents
mdkir exemplo
cd exemplo
mkdir exemplo-fullstack
cd exemplo-fullstack
git init
ls -la
git status
nano exemplo.md
cat exemplo.md
git status
git add .
git status
git rm --cached exemplo.md
git status
git commit -m "meu primeiro commit"
git add .
git status
git commit -m "meu primeiro commit"
git branch
git checkout -b dev
git status
ls -la
git branch
nano exemplo2.md
ls -la
git add .
git commit -m "meu segundo commit"
git checkout master
ls -la
git merge dev
git branch -d dev
git branch
history
