## Inicializando um repositório

Ao criar um repositório no [Gitlab](http://gitlab.com/), [Github](http://github.com/) ou ainda no [BitBucket](https://bitbucket.org) a plataforma nos oferece duas opções.

1. Criar um repositório onde não existe nada.
2. Criar um repositório onde o código já existe.

Para o caso 1.

Inicializando um projeto completamento do zero, crie o diretório do projeto e inicialize este projeto com o comando `git init`, por exemplo.

```
mkdir meu-novo-projeto
cd meu-novo-projeto
git init
```

Ao executar o comando `git init`, o retorno será algo do tipo:

> Importante lembrar que a saída deverá ligeriamente diferente para cada um, pois depende de Sistema Operacional e usuário.

```
Initialized empty Git repository in /home/rafael/meu-novo-projeto/.git/
```

Para o caso 2.

Inicializando um projeto com código já existente é necessário também inicializar o repositório com o comando `git init`, mas agora é necessário adicionar o seu repositório remoto ao seu computador com o comando:

```
git remote add origin git@gitlab.com:raffaeldutra/meu-novo-projeto.git
```

Quando executar o comando, não haverá um retorno no terminal.

Para listar os repositórios remotos, utilize o comando:

`git remote -v`

```
origin	git@github.com:raffaeldutra/meu-novo-projeto.git (fetch)
origin	git@github.com:raffaeldutra/meu-novo-projeto.git (push)
```

## Configuração do repositório

Todo novo repositório deverá ser criado algumas configurações, como por exemplo, quem é a pessoa que está criando código. Estas informações serão apresentadas no repositório para sabermos quem criou ou modificou algum arquivo.

Configure o seu email.
`git config user.email "raffaeldutra@gmail.com"`

Configure seu nome.
`git config user.name "Rafael Dutra"`

> Cuidado ao utilizar a opção --global, pois todos seus projetos irão ter o mesmo usuário e email.