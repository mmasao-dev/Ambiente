# Git

## O que �

Iremos abordar apenas um resumo, quanto a historia do git sugiro ler algum livro

O git foi criado para a gest�o de versionamento do software, para que cada colaborador possa contribuir simultaneamente no mesmo projeto, tendo o minimo de divergencias na estrutura do codigo.

Podemos ter o git apenas localmente para que voc� controle as suas vers�es de c�digos.

Para que o codigo seja compartilhado com mais colaboradores � necess�rio que haja um reposit�rio git, podemos citar o gitlab, gitbucket, github dentre outros.

Utilizaremos o github como exemplo.

## Github

Crie a conta do github seguindo as instru��es

github.com/signup

<i>
    <b>

* ***Entre com seu e-mail***
* *Crie uma senha**

* **Confirme sua conta no e-mail enviado pelo sistema.***

### *Enviar Commits*

*Para subir seus c�digos locais para o reposit�rio remoto s�o utilizados 2 protocolos, via https ou ssh.*

### *Https*

*Neste protocolo se utiliza o https onde seus commits s�o enviados atrav�s de login e senha do github*

 *Ser� solicitado o nome do seu usu�rio e a senha toda a vez que o commit for realizado.*

## *SSH-key*

*Neste m�todo o commit ser� enviado automaticamente, sem a necessidade de digitar seu usu�rio e senha a cada commit.*

*Antes de adicionar a chave, � necess�rio pegar a chave ou criar uma para o uso .*

*Eu recomendo criar uma chave espec�fica para cada uso.*

*Se voc� j� possui uma chave rsa, verifique o arquivo id_rsa.pub est� no seu diret�rio .ssh*

> *ls -lah ~/.ssh/*

*Caso j� possua e n�o queira gerar uma outra chave passe para a parte de adicionar a chave ao reposit�rio github.*

### *Gerando uma ssh-key*

*Verifique se o pacote openssh-client*

 *ssh-V*

 *Caso n�o possuo instale o pacote com o comando*

> *sudo apt install openssh-client -y*

*Gerar a chave personalizada*

> *ssh-keygen -t rsa -b 4096 -f ~/.ssh/id_rsa_nome_personalizado -C "seu_email@seu.dominio"*

*Entre com uma senha, n�o � obrigat�rio.*

*No caso de duvida quanto aos parametros acesse o*

 *https://man.openbsd.org/ssh-keygen.1*

*Ler sua chave publica e adicionar ao github.
leia o arquivo gerado pela ssk-key `<b>`.pub`</b>`*

> *cat ~/.ssh/idrsa_nome_personalizado.pub*

*Copie todo o codigo*

*exemplo:
ssh-rsa iasbq321sSDFDAGFojads... MA3dcgV34aaf==seu_email@seu.dominio*

*Abra o github e v� nas configura��es, em SSH and GPG keys adione uma nova chave*

*https://github.com/settings/keys*

*Sincronizar o ssh*

*Verifique se o ssh-agent est� rodando*

> *eval $(ssh-agent -s)*

*Adicione a chave privada*

> *ssh-add ~/.ssh/id_rsa_nome_personalizado*

 *Caso tenha colocado senha o agente vai solicitar ela.*

*Testar a conex�o*

> *ssh -T git@github.com*

 *The authenticity of host 'github.com (20.201.28.151)' can't be established.
    ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
    This key is not known by any other names*

*Ser� solicitado a adi��o de seguran�a do ssh remoto (! Leia sobre fingerprint)*

 *Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
    Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.*

*Se estiver ok a mensagem abaixo ser� exibida*

 *Hi Conta_git_hub! You've successfully authenticated, but GitHub does not provide shell access.*

### *Configura��o Git local*

*Realize a configura��o do git para identifica��o*

> *git config --global user.name "Fulano de Tal"*

> *git config --global user.email seuemail@seudominio*

*Estas configuira��es s�o necess�rio para identificar o autor no caso de se conectar com algum reposit�rio git.*

*`<u>` A conex�o entre o seu reposit�rio local e o repositorio remoto est� configurado.*

---
