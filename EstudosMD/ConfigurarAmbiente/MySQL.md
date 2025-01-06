# Passos para Instalar o MySQL

## 1. Obter Permissões de Superusuário
Primeiro, você precisa obter permissões de superusuário para executar os comandos de instalação.

```bash
sudo su
```
O comando `sudo su` permite que você se torne o usuário root e tenha permissões administrativas no sistema.

## 2. Instalar o Repositório APT do MySQL
Baixe [aqui](https://dev.mysql.com/downloads/repo/apt/) e instale o repositório MySQL APT, que é necessário para configurar os pacotes de instalação do MySQL.


```bash
dpkg -i mysql-apt-config_0.8.33-1_all.deb
```

O comando `dpkg -i` instala o arquivo .deb do repositório APT do MySQL. Isso permite que você baixe e instale o MySQL diretamente dos repositórios oficiais.

<br>

Ao executar esse comando, uma tela de configuração aparecerá. Escolha a opção para instalar o MySQL Server & Cluster e selecione a versão MySQL 8.0.

## 3. Atualizar a Lista de Pacotes
Após adicionar o repositório, você deve atualizar a lista de pacotes disponíveis para garantir que os pacotes mais recentes sejam acessíveis.

```bash
apt-get update
```

O comando `apt-get update` atualiza a lista de pacotes e repositórios disponíveis no seu sistema.

## 4. Instalar o MySQL Server
Agora, você pode instalar o MySQL Server no seu sistema.

```bash
apt-get install -y mysql-server
```

O comando `apt-get install -y mysql-server` instala o MySQL Server de maneira automatizada. O -y permite que a instalação seja feita sem pedir confirmação ao usuário.

## 5. Acessar o MySQL
Após a instalação, você pode acessar o MySQL utilizando o cliente de linha de comando:

```bash
mysql -u root -p
```

O comando `mysql -u root -p` permite que você acesse o MySQL com o usuário root. O sistema pedirá a senha de root para autenticação.

## 6. Testar se o MySQL Está Funcionando
Para verificar se a instalação foi bem-sucedida e o MySQL está funcionando corretamente, você pode listar os bancos de dados existentes.

```bash
show databases;
```

O comando `show databases;` exibe todos os bancos de dados presentes no MySQL, confirmando que o servidor está em funcionamento.

## 7. Sair do MySQL
Para sair do cliente MySQL, basta digitar o comando abaixo e pressionar Enter.

```bash
quit
```

O comando `quit` encerra a sessão atual do MySQL e retorna ao terminal do sistema operacional.
