# my-api-laravel
API Example using Laravel and PostgreSQL

## Install
```shell 
git clone https://github.com/01viniciusmelo/my-api-laravel.git
cd my-api-laravel
composer install
```

## Create table PostgreSQL
```sql
CREATE TABLE pessoa (
	id int4 NOT NULL,
	nome varchar(30) NULL,
	email varchar(50) NULL,
	dt_cadastro date NULL DEFAULT now(),
	CONSTRAINT pessoa_pkey PRIMARY KEY (id)
)
WITH (
	OIDS=FALSE
) ;
```

## Configure Virtual Hosts
```xml
<VirtualHost *:80>
    DocumentRoot "CAMINHO_PARA_PASTA_DA_API"
    ServerName laravel.exemple
</VirtualHost>
```
