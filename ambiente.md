# Criando ambiente 

## Conhecimentos necessários

- Linux (ubuntu)
- GIT
- Markdown 

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

### Windows Terminal
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

### Configuração Git 

Realize a configuração do git para identificação

> git config --global user.name "Fulano de Tal"

> git config --global user.email seuemail@seudominio

Estas configuirações são necessário para identificar o autor no caso de se conectar com algum repositório git.

---



