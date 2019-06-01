## Adicionando arquivos ao repositório local

Todo arquivo criado ou modificado, deve ser adicionado ao seu repositório local com o comando `git add`.

A sintaxe do comando `git add` é a seguinte:

`git add [OPÇÕES] arquivo1 arquivo2 arquivo3 ...`

Crie o primeiro arquivo chamado `readme.md` com o seguinte conteúdo:

```
# Primeiro titulo

Iniciando a documentação do projeto
```

Adicione o arquivo com `git add`

`git add readme.md`

Verifique o status do git com o comando:

`git status`

```bash
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	readme.md

nothing added to commit but untracked files present (use "git add" to track)
```

Temos arquivos com status de `Untracked files`, estes são os arquivos que não estão ainda sendo rastreados pelo versionamento.

Faça o commit deste arquivo com o comando:

`git commit -m 'Meu primeiro commit'`

```bash
[master (root-commit) b9deae4] Meu primeiro commit
 1 file changed, 3 insertions(+)
 create mode 100644 readme.md
```