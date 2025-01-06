# udemySpringReactEtc
## Configurando ambiente java (Linux)

Abaixo estão os comandos para adicionar o repositório, instalar o Java e verificar a instalação no ambiente Linux (Ubuntu).

### 1. Adicionar o Repositório PPA para o Java
Este comando adiciona o repositório PPA (Personal Package Archive) do **linuxuprising** que contém as versões mais recentes do Java.

```bash
sudo add-apt-repository ppa:linuxuprising/java
```

### 2. Atualizar a Lista de Pacotes
Após adicionar o repositório, é importante atualizar a lista de pacotes para garantir que o sistema tenha as versões mais recentes.

```bash
sudo apt-get update
```

### 3. Buscar as Versões do Java Disponíveis
Este comando exibe as versões do Java disponíveis no repositório, o que pode ser útil para escolher a versão que você deseja instalar.

```bash
sudo apt-cache search oracle-java
```

### 4. Instalar o Java (Exemplo com Java 17)
Instala a versão Oracle Java 17. Substitua oracle-java17-installer por outra versão, caso necessário.

```bash
sudo apt install -y oracle-java17-installer
```

### 5. Verificar a Versão do Java Instalado
Após a instalação, você pode verificar se o Java foi instalado corretamente com este comando, que exibe a versão atual do Java.

```bash
java --version
```

### 6. Verificar a Versão do Compilador Java (javac)
Este comando exibe a versão do compilador Java, útil para garantir que a instalação do JDK (Java Development Kit) está correta.

```bash
javac --version
```