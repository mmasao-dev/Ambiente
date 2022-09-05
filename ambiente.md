# Criando ambiente 

## Introdu��o
Dizem que o melhor ambiente para desenvolvimento seguro � usar um sistema operacional baseado no linux como a distro Ubuntu�, que � uma das preferidas pelo ambiente amig�vel

Mas como a maioria dos usu�rios s�o acostumada ao sistema Windows, sente muitas dificuldades ao migrar totalmente de plataforma e normalmente acaba voltando para o windows.

Existem solu��es em que podemos utilizar para criar o ambiente de desenvolvimento, como termos um dual boot na m�quina com windows e linux ou utilizando git, tortoise-git e vscode. 

Para um ambiente de desenvolvimento utilizando o melhor de ambos os sistemas, vamos montar o ambiente baseado no wsl2 e vscode, onde teremos o beneficio do linux sem alterarmos de sistemas. 

## Objetivo 

Habilitar o usu�rio a configurar um ambiente seguro de desenvolvimento no sistema Windows usando o Wsl.


## Resumo 
Este documento tem os passos basicos de uma cria��o de ambiente de desenvolvimento dentro do windows utilizando linux atrav�s do microsoft wsl2 e editor vscode .

Ser� abordado a instala��o do wsl2, vscode, windows terminal.

O documento est� escrito em markdown para facilitar a compatibilidade entre plataformas.

No final teremos uma ambiente de desenvolvimento windows 

## Conhecimentos necess�rios

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

    A instala��o do wsl2 pode ser seguida no site da microsoft e seguir o passo a passo e n�o ser� abordada 

    https://docs.microsoft.com/pt-br/windows/wsl/install


Instalando software iniciais.

Acesse microsoft Store para a distro e o windows terminal

### Ubuntu
 Baixe a distribui��o ubuntu - pode ser selecionado a instala��o da vers�o do ubuntu 18.02 LTS at� a recente vers�o 22.04 LTS, de preferencia para a mais recente. 

 Ao final da instala��o ser� necess�rio configurar seu usu�rio 

 ser� apenas ser� solicitado o nome de usu�rio e a senha.

 ap�s finalizar a instala��o o terminal bash do ubuntu ser� aberto.

 Neste ponto j� temos uma distro linux rodando na sua m�quina.

Atualize o ubuntu com o comando 

> sudo apt update & apt upgrade -y 

### Windows Terminal (Opcional)

Ao utilizar o Wsl, ser� aberto um terminal bash, caso precise utilizar um segundo terminal, ao abrir o linux ser� aberto uma nova janela.
O Windows terminal pode melhorar o uso, onde teremos apenas uma janela e os terminais estar�o separados por abas.

Baixe o Windows terminal - necess�rio caso vc queira usar mais de uma instancia do ubuntu, ela � compativel com os terminais shell windows e linux.

Configurando Terminal Windows

Abra o terminal windows, por padr�o o prompt de command ser� aberto.

V� em configura��es (ctrl+,) em inicializa��o selecione o perfil padr�o como ubuntu 

Verifique em perfis se o perfil do sistema foi criado. 

Acesse o site da microsoft para mais configura��es 

https://docs.microsoft.com/pt-br/windows/terminal/install

### Vscode

Baixe o editor de texto vscode atrav�s do site, � possivel baixar ele atrav�s o store tambem.

Este editor de texto gratuito � uma ferramenta poderosa para desenvolvimento. 

Caso tenha duvidas para cria��o do ambiente acesse

https://docs.microsoft.com/pt-br/windows/wsl/setup/environment?source=recommendations

--- 
## Git 

O git j� vem instalado por padr�o nesta vers�o do ubuntu n�o sendo necess�rio realizar o download dele. 

Caso tenha baixado uma outra vers�o da distro realize a instala��o do git 

> sudo apt update & apt install git





