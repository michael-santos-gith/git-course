# Iniciando com o Git e Github. #

Em poucas palavras o Git é um sistema de controle de versão de código aberto criado por Linus Torvalds criador do Kernel Linux, o Git possui uma arquitetura distribuída DVCS (Sistema de Controle de Versão Distribuído).

## Instalando ##

Para poder usar o Git é necessário sua instalação, existem várias maneiras, abaixo irei listar algumas delas.

## Instalação no Linux

Geralemente as istribuições Linux já vem com o Git, basta conferir digitando no terminal `git --version`.

Caso aparece um erro ou alguma outra menssagem o git não deve está instalado, aqui mostrarei como instalar em distribuições *.deb* como Debian, Ubuntu, Mint entre outras, ao final deixarei links para instalação em outras distros que são bastante populares também.

`$ sudo apt install git`

### Instalação em outras distros

**Fedora**  
`sudo yum install git` ou 
`sudo dnf install git`

**Gentoo**  
`sudo emerge --ask --verbose dev-vcs/git`

**Arch Linux**  
`sudo pacman -S git`

**OpenSUSE**  
`sudo zypper install git`

### Instalando no Windows

A instalação no Windows é bem simples basta ir ao (http://git-scm.com/download/win/) e escolher sua versão que pode ser 32 ou 64bits, o download começará automaticamente. 

### Instalação no Mac

Há varias opções para instalar o Git no Mac, nesse exemplo vou usar o Homebrew. Instale o Homebrew se você ainda não o tiver, depois:

`$ brew install git`

## Configurações básicas

Depois da instalação do Git algumas configurações devem ser feitas, como a identificação do usuário. Como será mostrado abaixo:

`git config --global user.name "seu_nome"`  
`git config --global user.email "seu_email"`

Exemplo:

`git config --global user.name "Michael Santos"`  
`git config --global user.email "maiconxandroid@gmail.com`

Há várias outras configurações que você pode fazer como, do editor, do diff e cor há também a possibilidade de verificar todas as configurações do git com o comando:

`git config --list`

## Comandos Básicos

A seguir alguns commando iniciais do Git:

1.*Clone*:criauma copia do repositório na sua máquina.`git clone`  
2.*Pull*:faz uma sincronização do seu repositório local com o online.`git pull`  
3.*Push*:após as alterações no seu repositório local faz o envio dessas alterações para o repositório online.`git add` seguido de `git commit -m "comentário"` e `git push`  

## **Iniciando**

Vamos iniciar um repositório local com o git, vá na pasta do projeto e digite **$ git init** .

*#Iniciar o repositório*  
`git init`

*#Adiciona todos arquivos existentes*  
`git add`

*#Cria o primeiro commit no histórico de versões*  
`git commit -m "Inicial commit"`

## Clonando projeto

Para iniciar um projeto no GitHUb ou colaborar com um, assim sendo esse projeto local também, é necessário a clonagem do projeto no seu computador. Usa-se o comando `$ git clone url-do-projeto`.

### Verificando status do repositório

Para verificar o status do repositório é só rodar o comando `$ git status`, se ouve alguma criação, modificação ou remoção de arquivo o __git status__ irá notificar na tela.

### Adicionando e/ou modificando arquivos

Todas as alterações no repositório local devem ser adicionadas no git, existe duas formas de se fazer isso:
com o **$ git add .** ou **$ git add <caminho_do_arquivo&gt;**. Na primeiro opção o ponto indica o diretório atual e que todos os arquivos serão mandados para o git, já na segunda mandará um arquivo por vez e está é a opção mais aconselhável, já que ao usar a primeiro você mandará todos os arquivos pessoais, de banco de dados, configurações e outros arquivos sensíveis.