# data-integration

O objetivo do projeto é criar uma API para carregar e integrar dados a partir de informações  de arquivos .csv.
Após a carga, é possível fazer consultas desses dados na API.
O projeto conta com alguns testes.

### Execução
Para executar o projeto é necessário ter o MongoDB local (localhost:27017) ou alterar as configurações de BD no arquivo application.properties.

Executar o arquivo para iniciar o serviço:
  
    java -jar data-integration-1.0.jar 

Foram criados 3 serviços REST:

    localhost:8080/companies/load

    localhost:8080/companies/integration

    localhost:8080/companies/search?name=DIRECTV&zip=38006

Na busca, ambos devem ser colocados como parâmetro, porém apenas um dos dois ou ambos devem estar preenchidos. É possível pesquisar por name e zip, name ou zip, sendo que o name retorna a partir de parte da palavra.

