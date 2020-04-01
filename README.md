# README

Esta aplicação é uma aplicação rails de um conversor de moedas, na qual utilizo para treinar minhas habilidades com rails

O projeto está dockerizado por isso para rodar basta executar: 

```docker
docker-compose build
docker-compose up -d
```

Para testar o serviço de conversão, basta que você execute os seguintes comandos: 

Entre no console do Rails
```docker
docker-compose run bundle exec rails c
```
Depois disso chame o serviço diretamente no console, exemplo:
``` ruby
exchange = ExchangeService.new('USD','BRL',2).perform
```
