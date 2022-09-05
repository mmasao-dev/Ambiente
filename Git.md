# Git

## O que é

Iremos abordar apenas um resumo, quanto a historia do git sugiro ler algum livro

O git foi criado para a gestão de versionamento do software, para que cada colaborador possa contribuir simultaneamente no mesmo projeto, tendo o minimo de divergencias na estrutura do codigo.

Podemos ter o git apenas localmente para que você controle as suas versões de códigos.

Para que o codigo seja compartilhado com mais colaboradores é necessário que haja um repositório git, podemos citar o gitlab, gitbucket, github dentre outros.

Utilizaremos o github como exemplo.

## Github

Crie a conta do github seguindo as instruções

github.com/signup

<i>
    <b>

* ***Entre com seu e-mail***
* *Crie uma senha**

* **Confirme sua conta no e-mail enviado pelo sistema.***

### *Enviar Commits*

*Para subir seus códigos locais para o repositório remoto são utilizados 2 protocolos, via https ou ssh.*

### *Https*

*Neste protocolo se utiliza o https onde seus commits são enviados através de login e senha do github*

 *Será solicitado o nome do seu usuário e a senha toda a vez que o commit for realizado.*

## *SSH-key*

*Neste método o commit será enviado automaticamente, sem a necessidade de digitar seu usuário e senha a cada commit.*

*Antes de adicionar a chave, é necessário pegar a chave ou criar uma para o uso .*

*Eu recomendo criar uma chave específica para cada uso.*

*Se você já possui uma chave rsa, verifique o arquivo id_rsa.pub está no seu diretório .ssh*

> *ls -lah ~/.ssh/*

*Caso já possua e não queira gerar uma outra chave passe para a parte de adicionar a chave ao repositório github.*

### *Gerando uma ssh-key*

*Verifique se o pacote openssh-client*

 *ssh-V*

 *Caso não possuo instale o pacote com o comando*

> *sudo apt install openssh-client -y*

*Gerar a chave personalizada*

> *ssh-keygen -t rsa -b 4096 -f ~/.ssh/id_rsa_nome_personalizado -C "seu_email@seu.dominio"*

*Entre com uma senha, não é obrigatório.*

*No caso de duvida quanto aos parametros acesse o*

 *https://man.openbsd.org/ssh-keygen.1*

*Ler sua chave publica e adicionar ao github.
leia o arquivo gerado pela ssk-key `<b>`.pub`</b>`*

> *cat ~/.ssh/idrsa_nome_personalizado.pub*

*Copie todo o codigo*

*exemplo:
ssh-rsa iasbq321sSDFDAGFojads... MA3dcgV34aaf==seu_email@seu.dominio*

*Abra o github e vá nas configurações, em SSH and GPG keys adione uma nova chave*

*https://github.com/settings/keys*

*Sincronizar o ssh*

*Verifique se o ssh-agent está rodando*

> *eval $(ssh-agent -s)*

*Adicione a chave privada*

> *ssh-add ~/.ssh/id_rsa_nome_personalizado*

 *Caso tenha colocado senha o agente vai solicitar ela.*

*Testar a conexão*

> *ssh -T git@github.com*

 *The authenticity of host 'github.com (20.201.28.151)' can't be established.
    ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
    This key is not known by any other names*

*Será solicitado a adição de segurança do ssh remoto (! Leia sobre fingerprint)*

 *Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
    Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.*

*Se estiver ok a mensagem abaixo será exibida*

 *Hi Conta_git_hub! You've successfully authenticated, but GitHub does not provide shell access.*

### *Configuração Git local*

*Realize a configuração do git para identificação*

> *git config --global user.name "Fulano de Tal"*

> *git config --global user.email seuemail@seudominio*

*Estas configuirações são necessário para identificar o autor no caso de se conectar com algum repositório git.*

*`<u>` A conexão entre o seu repositório local e o repositorio remoto está configurado.*

---
