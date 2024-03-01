# Atualização do Servidor e Implantação de Aplicação Web

Este script automatiza o processo de atualização do seu servidor e implantação de uma aplicação web. 
## Uso

1. **Atualizar o Servidor:**
 Execute os seguintes comandos para atualizar o seu servidor:

```bash
 echo "Atualizando o Servidor"
 apt-get update
 apt-get upgrade -y
 ```

2. **Instalar Apache e Unzip:**
 Instale o servidor web Apache e a ferramenta unzip com os seguintes comandos:

```bash
 apt-get install apache2 -y
 apt-get install unzip -y
 ```

3. **Baixar e Implantar a Aplicação:**
 Baixe os arquivos da aplicação do GitHub e implante-os no servidor web:

```bash
 echo "Baixando e copiando os arquivos da aplicação ..."

cd /tmp
 wget https://github.com/denilsonbonatti/linux-site-dio/archive/refs/heads/main.zip
 unzip main.zip
 cd linux-site-dio-main
 cp -R * /var/www/html/
 ```
