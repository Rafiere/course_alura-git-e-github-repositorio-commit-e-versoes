# AULA 01 - CONTA NO GITHUB

Nessa aula, aprenderemos sobre o GitHub.

Praticamente todas as vagas relacionadas à tecnologia pedem que o candidato saiba mexer com o sistema de versionamento Git.

O Git garante o versionamento de código, assim, podemos acessar várias versões de um determinado código.

Com o GitHub, podemos colocar vários códigos em repositórios, e esses repositórios ficarão disponíveis na nuvem para serem acessados.

Se digitarmos o link `repo.new` no navegador, seremos redirecionados para a página de criação de um novo repositório no GitHub.

Normalmente, o arquivo `README.md` possui informações sobre a configuração do projeto.

O formato Markdown é utilizado para documentações posts de blog e etc.

# AULA 02 - COMMIT, VSCODE E EQUIPE

Um `commit` é um envio de arquivos que fazemos, é como se criássemos um **registro do código naquele determinado momento**.

Podemos adicionar colaboradores em um repositório do GitHub. Quando adicionamos um colaborador, ele pode commitar no projeto e atualizar os arquivos que estão lá.

# AULA 03 - TRABALHANDO LOCALMENTE

## CLONANDO UM REPOSITÓRIO

O GitHub é um site que foi criado para **facilitar o uso do Git**.

O comando `git clone https://github.com/nome-do-usuario/nome-do-repositorio.git` permite que clonemos o repositório do projeto.

O comando `git log` permite que visualizemos o log dos commits do projeto de forma extensa.

O comando `git log --oneline` exibe todos os repositórios do projeto de forma resumida.

Quando realizamos o clone do projeto através do comando `git clone`, temos **todo o histórico de commits do projeto**.

## GIT STATUS, COMMIT E PUSH

O comando `git status` exibe o status dos arquivos que estão sendo versionados pelo Git.

O comando `git commit index.html -m "feat: adding index.html"` permite que criemos um commit localmente com a mensagem `feat: adding index.html`.

Se utilizarmos o comando `git commit . -m "mensagem do commit"`, commitaremos todas as alterações que foram feitas no projeto ao mesmo tempo.

O comando `git push origin main` permite enviarmos para a branch `main` do repositório remoto `origin`.

O `git diff` é a diferença entre dois commits.

Se utilizarmos o comando `git restore --source hash-do-commit .`, a aplicação voltará para o estado atual desse commit.

Caso queiramos que apenas um arquivo sofra o `restore`, basta utilizarmos o comando `git restore --source hash-do-commit nome-do-arquivo`.

## GIT LOG

Se utilizarmos o comando `git log --author="user_name"`, veremos todos os autores de um determinado commit.

Se utilizarmos o comando `git log --since=1.month.ago --until=1.day.ago`, veremos as informações do commit desde um mês atrás até um dia atrás.

Se utilizarmos o comando `git log --pretty="format:%h %s"`, podemos exibir o `hash` do commit, seguido com a mensagem de cada commit.

## CLONANDO BRANCHS ESPECÍFICAS

Se utilizarmos o comando `git clone -branch nome-da-branch repositorio`, conseguimos clonar uma branch específica de um repositório.

# AULA 04 - ADICIONANDO ARQUIVOS

## GIT ADD

Para adicionarmos apenas uma modificação para o commit, podemos utilizar o comando `git add nome-do-arquivo`, após isso, podemos utilizar o comando `git commit -m "mensagem-de-commit"` e o commit será feito apenas com esse arquivo.

Se utilizarmos o comando `git add .`, todas as modificações realizadas serão ouvidas, assim, podemos apenas utilizar o comando `git commit -m "mensagem-de-commit"` para commitarmos todas as modificações no arquivo.

# AULA 05 - RAMIFICAÇÕES E MERGE

## BRANCH

O `main`, ou `master`, normalmente, são os locais em que o projeto principal está localizado. Em cenários reais, trabalhamos com `branchs`, que são ramificações do código principal.

O comando `git checkout -b nome-da-branch` permite a criação de uma branch localmente. Essa branch será criada com base em **todo o código da branch em que estávamos anteriormente**.

O comando `git switch main` permite que mudemos para a branch `main`.

## MERGE

O `merge` consiste em juntarmos o código de duas `branchs` em apenas uma.

O comando `git branch` exibe todas as `branchs` que estão disponíveis no projeto.

Se utilizarmos o comando `git merge nome-da-main-que-queremos-juntar`, estamos realizando um `merge`, ou seja, estamos juntando o código da `branch` em que passamos o nome como argumento na `branch` em que estamos no momento.
