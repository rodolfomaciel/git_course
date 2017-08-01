Forma do git armazenar dados
[!Snapshots dos dados](https://git-scm.com/book/en/v2/images/snapshots.png)


Tres estagios do versionamento git
[!Estagios do Versionamento](https://git-scm.com/book/en/v2/images/areas.png)


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
[!Ciclo de trabalho](https://git-scm.com/book/en/v2/images/lifecycle.png)
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

