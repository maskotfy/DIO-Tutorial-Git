## Criando um repositório e aplicando o primeiro commit pelo Git Bash. 

Um pequeno projeto de Tutorial para aplicar meus conhecimentos adquiridos no curso de Git pela Dio. 



#### Passo 1 - Abrindo o Git Bash

- Abra o disco local (C:)
- Clique com o **botão direito** no disco local e em seguida clique em "Git Bash Here". Esse processo irá iniciar o Git Bash no seu diretório (C:)



#### Passo 2 - Criando as pastas para o repositório

- Com o Git Bash aberto, vamos criar uma pasta com o nome **"work"**, onde será o diretório do nosso primeiro repositório. 

ps: "work" é um nome que estou atribuindo para que facilite a didática. Renomeie como quiser.



- Utilize o comando a seguir para criarmos a primeira pasta: 

`mkdir work`



* Após criamos a primeira pasta, vamos navegar até ela utilizando o código: 

`cd work`



* Em seguida, no diretório **"work"**, vamos criar outra pasta que será nosso repositório. Utilize o seguinte código:

`mkdir repositorio`



* Para verificar se o repositório foi criado, utilize o código `ls` para listar o conteúdo no diretório **"work"**





#### Passo 3 - Criando repositório e iniciando o Git

* Agora vamos navegar até o repositório para que possamos iniciar o Git
* Digite o seguinte código: 

`cd repositorio`



* Após entrar no caminho **"/c/work/repositorio"**, vamos iniciar o Git possibilitando que ele crie um repositório vazio nesse destino. Utilize o seguinte código:

`git init`





**Passo 4 - Configurando e criando o primeiro arquivo do repositório**

* Antes de criar o primeiro arquivo do repositório, precisamos realizar uma configuração para que ele tenha um autor atrelado ao mesmo. Utilize o seguinte código: 

  `git config --global user.email "seuemail@email.com" `

  `git config --global user.name nickname`

  

  ps: Lembre se de usar o mesmo **e mail** e **nickname** que você utiliza para acessar o 

  GitHub.

- Após feita a configuração, vá até a pasta "**work/repositorio**" pelo seu disco local e crie um arquivo de sua preferência. Irei utilizar o nome **"Tutorial.md"** para facilitar a didática. 



- Após salvar **"Tutorial.md",** vamos aplicar o **"commit"** nesse arquivo utilizando os seguintes códigos:

`git add *`

``git commit -m "criando tutorial"``



obs1: O comando `git add ` é usado para enviar os arquivos que estão no estágio **"_Untracked_"**,  onde o Git não sabe da existência desse arquivo pois acabaram de ser criados, direto para**"_Staged_"**. Ou seja, onde estão sendo preparados para serem aplicados ao **"_commit_"**.



obs2: O "*" após o `add` é usado para pegar todos os arquivos do diretório e enviar para **"_Staged_"**.



obs3: Arquivos ***"Unmodified"***, ainda não sofreram modificação, caso altere algo nesse arquivo, ele muda para ***"Modified"*** . A razão disso é que o Git compara o **SHA1** dos arquivos e descobre que sofreu alguma alteração. 



obs4: A flag `-m` é usada para atribuir uma mensagem ao **commit** criado.