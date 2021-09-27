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

A instalação no Windows é bem simples basta ir ao (http://git-scm.com/download/win/){target="_blank"} e escolher sua versão que pode ser 32 ou 64bits, o download começará automaticamente. 
