# Instalando e configurando Oh-my-zsh

## Introdução

Como vamos utilizar o terminal bash, por que não utilizar um terminal mais pesonalizável. 

Istalaremos o ZSH como terminal no lugar do bash, ele é um poderoso teminal com suporte a vários plugins e temas que ajudarão muito na area de desenvolvimento. 

> sudo apt install zsh -y


## oh my ZSH

Instalado o Zsh, instalaremos o framework oh-my-zsh o qual irá gerenciar nossos plugins e temas.

Acesse o site 

    https://ohmyz.sh/

Vá em install oh-my-zsh

copie o comando e cole no terminal bash

sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

Ele irá baixar e automaticamente substiruir seu shell

Clique em sim para aceitar a troca do shell padrão 

    Looking for an existing zsh config...
    Using the Oh My Zsh template file and adding it to ~/.zshrc.

    Time to change your default shell to zsh:
    Do you want to change your default shell to zsh? [Y/n] 

## configurando 

Vamos editar o tema do zsh pelo oh-my-zsh <br>
Aqui usarei o nano

> nano ~./zshrc

### Temas
O tema padrão é o robbyrussell 
vá até a linha <br>

ZSH_THEME="robbyrussell" <br>

e altere para um tema de sua preferencia. 

para selecionar os temas já pré configurados pelo oh-my-zsh acesse o site <br>
https://github.com/ohmyzsh/ohmyzsh/wiki/Themes

escolha um deles e substitua o tema padrão

#### Temas Externos 
Além dos temas que o oh-my-zsh, temos a possibilidade de instalar temas externos. <br>

https://github.com/ohmyzsh/ohmyzsh/wiki/External-themes

para a instalação de temas externos é necessário acessar o repositório e seguir as instruções de cada desenvolvedor.

### Plugins

Para instalar plugins, vá até a linha 

plugins=(git)

e vá adicionado os plugins de sua preferencia. 
A lista de plugins pré configurados está em https://github.com/ohmyzsh/ohmyzsh/wiki/Plugins

O plugin do git já vem por padrão.

Como os temas podemos instalar plugins externos tambem .<br>
https://github.com/ohmyzsh/ohmyzsh/wiki/External-plugins

Alterado o tema e instalado os plugins salve o arquivo.<br>
reinicie o shell zsh 

* <b> Antes de instalar o plugin, leia atentamente para que serve e os passos de sua instalação.

> source ~/.zshrc

#### Plugins usados no meu terminal 

- Git 
- ssh-agent
- zsh-autosuggestions 
- zsh-zyntax-highlightting 


