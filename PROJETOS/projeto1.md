# - RECEITA PARA CRIAR REPOSITÓRIOS - kali linux
## - MODO DE PREPARO - 
    1 - abra o terminal, utilize os comandos de diretórios para criar uma pasta para seu repositório do github.
    2 - vá até a pasta criada e utilize o comando "git init" para criar o seu  repositório dentro da pasta. Possibilitando a versionabilidade e gerenciamento do seu codigo.
    3 - utilize o comando "git config --global user.email/name 'nome ou email' para configurar seu nome de usuário e email.

### - COMMITS - criação e ciclo de vida
    1 - vá até a pasta do seu repositório e crie um arquivo com o final ".md" (markdown).
    2 - nesse arquivo, você escreverá as informações desejadas, o seu código.
    3 - utilize o comando "git status" para observar os arquivos "untracked" dentro da pasta do repositório.
    4 - utilize o comando "git add *", para modificar o estado do(s) arquivo(s) .md "untracked" que estão dentro da pasta para "staged".
    5 - utilize o comando "git commit -m 'mensagem'" para adicionar um commit no arquivo. Esse commit traz as informações das alterações feitas no arquivo, incluindo o nome do autor responsável. (OBS:. se o nome de usuário do github for diferente ao configurado no kali, então os commits serão representados com nome diferente no site do github).
    6 - utilize o comando "git status" novamente, para confirmar as alterações. Agora deverá aparecer que a "working tree" está "clean", ou seja, não há arquivos necessitando serem "commitados".
    7 - novamente, crie um arquivo com o final ".md" com nome de "README.md". Este arquivo irá carregar as informações sobre os objetivos do seu repositório e seus projetos.
    8 - utilize o comando "git add *" para mover o(s) arquivo(s) de "untracked" para "staged"
    9 - utilize o comando "git commit -m 'mensagem'" para adicionar um commit no arquivo.
    10 - utilize o comando "git status" para confirmar as alterações.

#### - REPOSITÓRIO LOCAL E REMOTO - interação, PUSH/PULL
     1 - crie um repositório no site do github.
     2 - aponte o repositório local para o remoto. È nescessário empurrar (push) o local para o remoto, primeiramente informe a origem. Utilize o comando "git remote add origin 'link do repositorio'".
     3 - utilize o comando "git remote -v" para listar os repositórios remotos cadastrados.
     4 - utilize o "git status" para verificar nenhuma pendência no repositório.
     5 - utilize o comando "git push origin master" para empurrar o repositório. Agora estão sincronizados ambos os repositórios, local(seuPC) e remoto(github).
     6 - caso algum arquivo esteja com conflitos de versionamento, voce precisara utilizar o comando "git pull origin master" para puxar de volta o arquivo do remoto para o local.
     7 - podem ocorrer problemas ao puxar, dependendo da configuracao do seu github. As vezes e necessario configurar a fundicao (merge) de arquivos, utilizando o comando "git config pull.rebase false" antes de utilizar o "pull".
     8 - na sequencia faca as edicoes no arquivo utilizando o comando "nano "nomedoarquivo.md", ou indo diretamente na pasta dentro do disco local.
     9 - utilize o comando "git add *" para adicionar os arquivos conflitantes para a area "staged"
     10 - agora faca um commit para concluir a fundicao dos arquivos e atualizar o repositorio, de forma a resolver os conflitos. Novamente, o repositorio local e remoto estao sincronizados.
