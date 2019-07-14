# firebird-php
Learning to create a PHP REST API using FIREBIRD as database.

## Instalando Firebird
Para instalar em um sistema Linux baseado em Ubuntu, devemos usar o seguinte comando:

` sudo apt-get install firebird3.0-server `

Suponhando que Apache2 + PHP já esteja instalado, não devemos instalá-los.

## Configurando Firebird no ambiente Apache2 + PHP

### Habilitando a extensão "php_interbase"

Abrindo o arquivo php.ini, localizado na pasta /etc/php/7.0/apache2/php.ini, devemos descomentar a seguinte linha:

` extension=php_interbase.so ` ou ` extension=php_interbase.dll `

De forma mais prática:

` sudo nano /etc/php/7.0/apache2/php.ini `

Usando Ctrl + W, procuramos por `interbase` e removemos o ';' da linha.

### Instalando a extensão php-firebird

Para a versão 7.0 do PHP, usamos o seguinte comando:

` sudo apt-get install php5-firebird `
