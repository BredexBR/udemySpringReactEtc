# Instalação do Eclipse via Spring Tools Suite
## 1. Instalar o eclipse
Clique [aqui](https://spring.io/tools) para acessar o site de instalação do eclipse.

## 2. Mova o arquivo para a pasta /opt
```bash
sudo mv spring-tool-suite-4-4.27.0.RELEASE-e4.34.0-linux.gtk.x86_64.tar.gz /opt
```

## 3. Abra a pasta opt
```bash
cd /opt/
```

## 4. Descompactar o arquivo
```bash
sudo tar zxvf spring-tool-suite-4-4.27.0.RELEASE-e4.34.0-linux.gtk.x86_64.tar.gz
```

## 5. Abra a pasta descompactada 
```bash
cd sts-4.27.0.RELEASE/
```

## 6. Execute o arquivo 
```bash
sudo ./SpringToolSuite4
```

## Opcional
Caso queira criar um arquivo executável no desktop:

```bash
sudo vi /usr/share/applications/stsLauncher.desktop
```

Insira dentro desse arquivo com a versão correta do Spring Tool: (aperte insert no teclado).

```bash
[Desktop Entry]
Name=Spring Tool Suite
Comment=Spring Tool Suite 4.27.0
Exec=/opt/sts-4.27.0.RELEASE/SpringToolSuite4
Icon=/opt/sts-4.27.0.RELEASE/icon.xpm
StartupNotify=true
Terminal=false
Type=Application
Categories=Development;IDE;Java;
```

E por fim acesse o executável no menu de aplicativos (Spring Tool Suite).