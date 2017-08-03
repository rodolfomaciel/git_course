# Branch

### Criando um novo branch ( ramo )
Para criar uma ramificação do seu código use o comando:
```
$ git branch <nome do ramo>
```

Criar e alternar para o novo branch:
```
$ git checkout -b <nome do ramo>
```

### Alternar entre branchs diferentes
Para mudar de um ramo para outro use o comando:

```
$ git checkout <nome do ramo>
```

### Mesclando branchs diferentes
Para mesclar as mudanças do ramo com o ramo principal faça:
```
$ git checkout master
$ git merge <nome do ramo>
```


### Excluindo um branch
Depois do git merge não há mais necessidade do ramo mesclado, por isso você faz:

```
$ git branch -d <nome do ramo>
```

### Resolvendo conflitos
Se por acaso houver algum conflito de mesclagem elas são exibidas com o comando:
```
$ git status
```

### Exibir branchs mesclados
Para exibir os ramos que já foram mesclados com o principal faça:
```
$ git branch --merged
```

### Outras opções de branch
Visualizar os ultimos commits em cada branch
```
$ git branch -v
```

Ramos que podem ser usados em desenvolvimento de projetos
- master
- develop
- topic
