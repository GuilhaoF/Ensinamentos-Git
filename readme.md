![git-githu-cover](https://user-images.githubusercontent.com/67026555/159383829-d0fde861-d0b9-48ab-840c-b25ebc72caa5.png)
### Comandos de Git no Terminal Para Iniciantes

Iniciando Git no Projeto

```bash
  git init
```

Verificar o Status

```bash
  git status
```

Adicione os arquivos nao rastreados(untracked)

```bash

  git add .  - adiciona todos os arquivos 
  git add nome_arquivo - adiciona arquivo especifico

```

Commitar(adicionar no repositorio local).

```bash

  git commit -m 

```
Comando para restaurar mudancas/modificacoes em determinado arquivo
Sem esta no stage area.

```bash
  git restore [nome do arquivo]

```

Trazendo de volta do stage area
Quando fizemos alguma alteracao e ela foi para nosso stage area 

```bash
  git restore --staged nomedoarquivo
```

Outra forma quando temos muitos arquivos
```bash
  git restore --staged .
```
Corrigindo ultimo commit 

```bash
 git commit --amend -m "nova mensagem"  
```

Podemos recuperar em nossos antigos commits um arquivo que foi modificado 
obs: HASH - primeiros caracteres da hash do commit

```bash
  git checkout HASH -- nomedoarquivo
```
Removendo arquivos nao rastreados 
- obs: vai deletar tudo que nao esta rastreado para sempre.

```bash
  git clean -f 
```

Revertendo um commit
obs: a cada commit subtrairemos -1,considere o commit atual como
```bash
  git revert HEAD ~ [numero do commit]
```

Outra forma mais simples seria com o comando :

```bash 
  git log --oneline
```
 e depois usar 

 ```bash 
 git revert [caracteres da hash]

 ```
Mostrar todas as modificacoes feitas em nossos arquivos que ja tinhamos feito em nosso repo

```bash 
 git diff
```
Mostrar as modificacoes dos arquivos no stage area e no repositorio 

```bash 
  git diff staged 
```
Deletar arquivos 

```bash
 git rm [nome do arquivo]
```
Renomear arquivos 

```bash 
 git mv [nome atual] [novo nome]
```
Movendo Arquivos
Podemos usar o comando `git mv`

```bash
  git mv [arquivo a mover] [diretorio]
  ex : git mv arquivo.txt  src/
```