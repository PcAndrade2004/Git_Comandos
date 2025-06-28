Aqui iremos adicionar comandos básicos do *Git*

<font color="#ff0000">🔄 Corrigir a mensagem do último commit

Copiar código</font>
* git commit -m "Adicionando arquivos" --amend

<font color="#ff0000">
🗑️ Apagar os últimos commits sem perder o conteúdo</font>
* Remove os Últimos 3 commits do histórico, mas mantém os arquivos alterados no stage.
```Texto
git reset --soft HEAD~3
```

<font color="#ff0000">🧩Editar ou reorganizar commits (modo interativo)</font>
* Abre um menu interativo no terminal para Editar, combinar, dividir ou reordenar os últimos 3 commits
```texto
git rebase -i HEAD~3
```

<font color="#ff0000">🔃 Cancelar arquivos do stage (remover do staging area)</font>
* Tira o arquivo da área de staging (área pronta para commit), **sem perder as alterações feitas**.
```Texto
git reset nome-do-arquivo
```

<font color="#ff0000">🧩Modo interativo de staging</font>
* Abre menu interativo no terminal para que u possa escolher quais arquivos ou partes de arquivos deseja adicionar.
```Texto
git add -i
```

![[Pasted image 20250626193317.png]]

<font color="#ff0000">🔍 Ver diferenças entre arquivos e commits</font>
* Mostra as **diferenças entre o conteúdo atual dos arquivos e o último commit**.  
  Ou seja: **o que você modificou, mas ainda não adicionou com `git add`**.
```Texto
git diff
```
