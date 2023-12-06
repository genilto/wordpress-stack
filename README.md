# wordpress-stack
Docker compose para rodar uma stack completa com wordpress

# README #

Este repositório possui as configurações necessárias para rodar uma stack wordpress utilizando o docker-compose.
Antes de rodar o compose, você deve configurar qual plataforma você deseja utilizar: x86 ou ARM.

É possível fazer isso apenas criando um link simbolico para o arquivo desejado:

X86
```
ln -s docker-compose-x86.yml docker-compose.yml
```

ou

ARM
```
ln -s docker-compose-arm.yml docker-compose.yml
```

# DOCKER COMPOSE #
Configurar o dados no .env baseado no example.env
Rodar o comando abaixo:

docker-compose up -d

# File and Folder Permissions

Change all directories recursively to 755:

$ find . -type d -exec chmod 0755 {} \;

Change all files recursively to 644:

$ find . -type f -exec chmod 0644 {} \;
