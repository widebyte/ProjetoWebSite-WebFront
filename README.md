# Projeto Quality Assurance | Challenge - Web Front
Neste projeto foi realizado uma automação com base em RUBY utilizando o seguinte site:
<a href="http://automationpractice.com/index.php">Automation Practice</a> 

As seguinte ações automatizadas foram:
* Um cadastro do usuário
* Login com sucesso
* Login em Branco
* Login Incorreto
* Obtenção de Reports

OBS: Abaixo, foi colocado o item de 'screenshots' para todos os testes na pasta Log, para obtenção dos relatórios dos testes.

## Ruby 
Neste projeto foi utilizado o Ruby para automação web. Foram utilizadas as seguintes gems: 
* gem "capybara"
* gem "cucumber"
* gem "rspec"
* gem "selenium-webdriver"
* gem "faker **Eu realizei a instalação dentro do projeto e no cadastrar_page.rb na linha 5, está como comentário, mas se quiserem rodar via API FAker com vários dados para cadastrar), apague a linha 6 e rode o comando cucumber -t @cadastrar e irá rodar em loop o cadastro no sistema com dados faker.**

## Capybara
O Capybara ajuda você a testar aplicativos da Web, simulando como um usuário real iria interagir com seu aplicativo. É independente do driver que está executando seus testes e vem com o suporte Rack :: Test e Selenium embutido. 

## Comandos do Projeto

OBS: JÁ ESTÁ COM CONFIGURADO COM UM USUÁRIO NÃO CADASTRADO. SÓ RODAR OS COMANDOS ABAIXO PARA RODAR OS TESTES POR COMPLETO!

**Para rodar o projeto por completo**
````
cucumber
````
**Rodar o projeto por tags**

* Rodar o projeto CADASTRAR
````
cucumber -t @cadastrar
````

* Rodar o projeto LOGAR
````
cucumber -t @login
````

## Rodar projeto com screenshots dos testes:
Os screenshots e o relatório se encontram na pasta Log. Após rodar o projeto por completo, rode o seguinte comando abaixo para obtenção dos reports:

````
* cucumber --format html --out=log/features.html
````
