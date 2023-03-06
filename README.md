<img src="http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=RED&style=for-the-badge"/>

# [delivery-api](https://github.com/delivery-api)
É um projeto que tem o objetivo de demostrar o uso do projeto *Spring Cloud*.

## Contextualização:
Micro service de pedido e entregas de produtos. 

*Cenário*: 
> O cliente entra na loja, compra determinado produto e pede para entregar em determinado endereço.<br/>
> A loja recebe o pedido e manda para o fornecedor.<br/>
> Fornecedor recebe o pedido, retorna o tempo de entrega para a loja. E realiza uma reserva de transporte, passando o endereço de origem e de destino.<br/> 
> Transportador recebe a requisição de transporte e devolve um voucher.

### [Contextos / Serviços](https://github.com/orgs/delivery-api/repositories):
- loja: gestão do pedido: apresenta o catálogo; realiza pedido; reserva um voucher
- transportador: gestão do voucher: gera o *voucher* para uma origem e destino
- fornecedor: gestão do catálogo: mantém o catálogo; executa os pedidos

### Estrutura 

<img width="375" alt="image" src="https://user-images.githubusercontent.com/42658870/223151534-2a7fcb52-93fc-49f4-bb9e-c364b1ad1b67.png">

## Tecnologias
- Spring Cloud 2022.0.1
- Spring boot 3.0.3
- java 17
- Maven 3.6.3
- MySQL 8.0
- Docker
- Lombok
- Papertrail
- Logback

#### *Done List*
- Microservice *loja* e *fornecedor*
- Eureka Server
- Config Server
- Config Repo (repositório com credenciais de acesso)
- Agregador de Log

#### *To Do List*
- Microservice *transportador*
- API Gateway
- Auth Server
- Micrometer Tracing, pois o *Spring Sleuth* não está disponível no Spring Boot 3. [info](https://docs.spring.io/spring-cloud-sleuth/docs/current/reference/html/README.html)
- Swagger
- Testes
- Sonar
- Jenkins







