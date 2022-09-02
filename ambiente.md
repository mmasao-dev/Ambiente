# Criando ambiente 

## Conhecimentos necess�rios

- Linux (ubuntu)
- GIT
- Markdown 

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

### Windows Terminal
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

### Configura��o Git 

Realize a configura��o do git para identifica��o

> git config --global user.name "Fulano de Tal"

> git config --global user.email seuemail@seudominio

Estas configuira��es s�o necess�rio para identificar o autor no caso de se conectar com algum reposit�rio git.

---



