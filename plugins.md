# Plugins para Omyzsh

## Git 

não necessário instalar o plugin, ele é nativo, apenas caso queira criar comandos personalizados via aliases. 

## ssh-agent

Toda as vezes que abrimos uma sessão no terminal linux, é necessário nós ativarmos o agente e caso necessário adicionar a private key. 

     eval "$(ssh-agent -s)"

     ssh-agent ~/.ssh/ID_CHAVE_REPOSITORIO

Para que não seja necessário iremos usar o plugin do ssh-agent. 

Como o plugin Git, este tambem não necessita de instalação, apenas a configuração dele 

Adicione após o plugins 

 # ohmyzsh ssh agent
zstyle :omz:plugins:ssh-agent agent-forwarding yes
zstyle :omz:plugins:ssh-agent identities rsa_sua_chave
zstyle :omz:plugins:ssh-agent lifetime 4h

## zsh-autosuggestions

Plugin para sugestão do comando digitado 

pagina no github </br>
https://github.com/zsh-users/zsh-autosuggestions

clone o repositório

    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

adicione em plugins o zsh-autosuggestions


## zsh-zyntax-highlightting

https://github.com/zsh-users/zsh-syntax-highlighting


Clone o repositório 

git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

adicione em plugins o zsh-highlightting

Adicionais do highlightting
    - Prezto
    - zgen
    - zplug
    - zplugin


Reinicie o omyzsh 

     source .zshrc
