Forma do git armazenar dados
![Snapshots dos dados](https://git-scm.com/book/en/v2/images/snapshots.png)


Tres estagios do versionamento git
![Estagios do Versionamento](https://git-scm.com/book/en/v2/images/areas.png)


Instalacao linux ubuntu
```
$ sudo apt-get install git-all
```
Configuracao do git

```
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
$ git config --global core.editor emacs

```
Obtendo ajuda
```
$ git help <palavra chave>
```

Iniciando um repositorio
```
$ git init (inicia um repositorio local)
$ git clone https://github.com/libgit2/libgit2 (copia um repositorio remoto)
```

Trabalhando no repositorio
![Ciclo de trabalho](https://git-scm.com/book/en/v2/images/lifecycle.png)
```
$ git status (determina que arquivos estao sendo rastreados)
$ git add * (marca todos os arquivos como rastreados)
```
Ignorando arquivos e pasta
-Crie um arquivo .gitignore e adicione os curingas de exclusao

Visualizando suas mudancas
```
$ git diff
$ git diff --staged (mostra todas as mudancas deste o ultimo commit)
```

Registrando no banco de dados
```
$ git commit -m "<mensagem do commit>"
$ git commit -a -m "<mensagem>" (pula a fase de stage)
```

Visualizando o historico de commits

O historico com a opcao p mostra o diff do commit
```
$ git log -p -2
$ git log --stat
$ git log --since=2.weeks
```

Desfazendo coisas

Refazer o ultimo commit incluindo as mudancas feitas depois dele
```
$ git commit --amend
```

O reset retira um determinado arquivo da area de selecao do commit
```
$ git reset HEAD CONTRIBUTING.md
```

Para ativar um arquivo novamente é só utilizar o comando checkout
```
$ git checkout -- CONTRIBUTING.md
```

Trabalhando com repositorios remotos

Exibindo os remotos
```
$ git remote
$ git remote -v
```

Adicionando um repositorio remoto
```
$ git remote add pb https://github.com/paulboone/ticgit
```

Obtendo as atualizacoes de um repositorio remoto especifico
```
$ git fetch pb
```

O comando pull sincroniza o repositorio principal com o local
```
$ git pull 
```

Empurrando seu trabalho local para o repositorio remoto
```
$ git push [remote-name] [branch-name]
$ git push origin master
```

Obtendo mais informacoes sobre o seu repositorio 
```
$ git remote show origin
```

Renomeando e removendo um repositorio remoto
```
$ git remote rename pb paul
$ git remote remove paul
```
Usando tags e anotacoes

```
$ git tag -a v1.4 -m "my version 1.4"
$ git tag
v0.1
v1.3
v1.4
$ git show v1.4
tag v1.4
Tagger: Ben Straub <ben@straub.cc>
Date:   Sat May 3 20:19:12 2014 -0700

my version 1.4

commit ca82a6dff817ec66f44342007202690a93763949
Author: Scott Chacon <schacon@gee-mail.com>
Date:   Mon Mar 17 21:52:11 2008 -0700

    changed the version number

$ git tag v1.4-lw
$ git push origin v1.5
```

Seus proprios atalhos

```
$ git config --global alias.co checkout
$ git config --global alias.br branch
$ git config --global alias.ci commit
$ git config --global alias.st status
$ git config --global alias.unstage 'reset HEAD --'
$ git config --global alias.last 'log -1 HEAD'
```
