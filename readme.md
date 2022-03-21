### Comandos de Git no Terminal Para Iniciantes

Iniciando Git no Projeto

```bash
  git init
```

Verificar o Status

```bash
  git status
```

Adicione os arquivos nao rastreados

```bash

  git add .  - adiciona todos os arquivos 
  git add nome_arquivo - adiciona arquivo especifico

```

Commitar(adicionar no repositorio local).

```bash

  git commit -m 

```
Comando para restaurar mudancas/modificacaoes em determinado arquivo
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

```
