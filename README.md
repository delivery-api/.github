# [delivery-api](https://github.com/delivery-api)
É um projeto que tem o objetivo de demostrar o uso do projeto *Spring Cloud*.

## Contextualização:
Micro service de pedido e entregas de produtos. 

*Cenário*: 
> O cliente entra na loja, compra determinado produto e pede para entregar em determinado endereço.<br/>
> A loja recebe o pedido e manda para o fornecedor.<br/>
> Fornecedor recebe o pedido, retorna o tempo de entrega para a loja. E realiza uma reserva de transporte, passando o endereço de origem e de destino.<br/> 
> Transportador recebe a requisição de transporte e devolve um voucher.

### Contextos / Serviços:
- loja: gestão do pedido: apresenta o catálogo; realiza pedido; reserva um voucher
- transportador: gestão do voucher: gera o *voucher* para uma origem e destino
- fornecedor: gestão do catálogo: mantém o catálogo; executa os pedidos

### Estrutura / endpoints:

(...)

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






