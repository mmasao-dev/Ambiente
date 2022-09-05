# Criando ambiente 

## Introdução
Dizem que o melhor ambiente para desenvolvimento seguro é usar um sistema operacional baseado no linux como a distro Ubuntu®, que é uma das preferidas pelo ambiente amigável

Mas como a maioria dos usuários são acostumada ao sistema Windows, sente muitas dificuldades ao migrar totalmente de plataforma e normalmente acaba voltando para o windows.

Existem soluções em que podemos utilizar para criar o ambiente de desenvolvimento, como termos um dual boot na máquina com windows e linux ou utilizando git, tortoise-git e vscode. 

Para um ambiente de desenvolvimento utilizando o melhor de ambos os sistemas, vamos montar o ambiente baseado no wsl2 e vscode, onde teremos o beneficio do linux sem alterarmos de sistemas. 

## Objetivo 

Habilitar o usuário a configurar um ambiente seguro de desenvolvimento no sistema Windows usando o Wsl.


## Resumo 
Este documento tem os passos basicos de uma criação de ambiente de desenvolvimento dentro do windows utilizando linux através do microsoft wsl2 e editor vscode .

Será abordado a instalação do wsl2, vscode, windows terminal.

O documento está escrito em markdown para facilitar a compatibilidade entre plataformas.

No final teremos uma ambiente de desenvolvimento windows 

## Conhecimentos necessários

- Windows 
- Windows Store
- Powershell
- Linux (ubuntu)
- GIT


## Softwares 
- WSL
- VsCode
- Windows Terminal


## wls2 

    A instalação do wsl2 pode ser seguida no site da microsoft e seguir o passo a passo e não será abordada 

    https://docs.microsoft.com/pt-br/windows/wsl/install


Instalando software iniciais.

Acesse microsoft Store para a distro e o windows terminal

### Ubuntu
 Baixe a distribuição ubuntu - pode ser selecionado a instalação da versão do ubuntu 18.02 LTS até a recente versão 22.04 LTS, de preferencia para a mais recente. 

 Ao final da instalação será necessário configurar seu usuário 

 será apenas será solicitado o nome de usuário e a senha.

 após finalizar a instalação o terminal bash do ubuntu será aberto.

 Neste ponto já temos uma distro linux rodando na sua máquina.

Atualize o ubuntu com o comando 

> sudo apt update & apt upgrade -y 

### Windows Terminal (Opcional)

Ao utilizar o Wsl, será aberto um terminal bash, caso precise utilizar um segundo terminal, ao abrir o linux será aberto uma nova janela.
O Windows terminal pode melhorar o uso, onde teremos apenas uma janela e os terminais estarão separados por abas.

Baixe o Windows terminal - necessário caso vc queira usar mais de uma instancia do ubuntu, ela é compativel com os terminais shell windows e linux.

Configurando Terminal Windows

Abra o terminal windows, por padrão o prompt de command será aberto.

Vá em configurações (ctrl+,) em inicialização selecione o perfil padrão como ubuntu 

Verifique em perfis se o perfil do sistema foi criado. 

Acesse o site da microsoft para mais configurações 

https://docs.microsoft.com/pt-br/windows/terminal/install

### Vscode

Baixe o editor de texto vscode através do site, é possivel baixar ele através o store tambem.

Este editor de texto gratuito é uma ferramenta poderosa para desenvolvimento. 

Caso tenha duvidas para criação do ambiente acesse

https://docs.microsoft.com/pt-br/windows/wsl/setup/environment?source=recommendations

--- 
## Git 

O git já vem instalado por padrão nesta versão do ubuntu não sendo necessário realizar o download dele. 

Caso tenha baixado uma outra versão da distro realize a instalação do git 

> sudo apt update & apt install git





