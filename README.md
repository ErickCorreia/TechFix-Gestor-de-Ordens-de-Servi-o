# TechFix — Gerenciador de Assistência Técnica

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![HTML](https://img.shields.io/badge/HTML-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)

## Sobre o Projeto
Este projeto resolve a dor de pequenas assistências técnicas que precisam organizar a entrada de hardwares e o status de manutenção.

## Como Executar

 Testes
- Execute: `./vendor/bin/phpunit tests`

1. Instale as dependências: `composer install`
## 1. composer install
O que faz: Lê o seu arquivo composer.json e baixa a pasta vendor/ com o PHPUnit.

Por que é vital: Sem isso, os testes não rodam e o PHP não vai achar as classes do seu projeto. É como baixar as peças antes de montar o motor.


2. Inicie o servidor: `php -S localhost:8000 -t src`
## 2. php -S localhost:8000 -t src
O que faz: Ativa o servidor embutido do PHP.

O parâmetro -t src: Esse é o "pulo do gato". Ele diz ao PHP que a "cara" do site está dentro da pasta src. Assim, quando você abrir o navegador, ele já lê o index.php direto.

3. Acesse: `http://localhost:8000`
## 3. ./vendor/bin/phpunit tests
O que faz: Chama o executor de testes que o Composer instalou.

O objetivo: Ele vai ler sua pasta tests e te dar o relatório (aquela barra verde) confirmando que o sistema está funcionando sem erros.

## OBS!!!
Quando você rodar o comando do servidor e abrir http://localhost:8000, se você seguiu o passo de separar o arquivo de cadastro, o fluxo será:

Você preenche o formulário.

O index.php envia para o cadastrar.php.

O cadastrar.php salva no database.sqlite e te joga de volta para a index.php com os dados atualizados na tabela.
