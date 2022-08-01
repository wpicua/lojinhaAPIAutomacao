# Lojinha API Automação

Esse é um repositório que contem a automação de alguns testes de API Rest de um software denominado Lojinha. Os sub-tópicos abaixo descrevem algumas decisões na estrutura do projeto.

## Tecnologias Utuilizadas

- Java
  https://www.oracle.com/java/technologies/downloads/#jdk18-windows
- JUnit
  https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-engine/5.9.0
- RestAssured
  https://mvnrepository.com/artifact/io.rest-assured/rest-assured/5.1.1
- Maven
  https://maven.apache.org/

## Testes Automatizados

- Testes para validar as partições de equivalência relacionadas ao valor do produto a lojinha, que estão vinculados diretamente a regra de negocio que diz que o valor do produto deve estar entre R$ 0,01 e R$ 7.000,00.

## Notas Gerais

- Sempre utilizamos a anotação Before Each para capturar o Token que será utilizado posteriormente nos métodos de testes.
- Armazenamos os dados que são enviados para a API através do uso de classes POJO.
- Criamos dados iniciais através do uso de classe Data Factore, para facilitar a criação e controle dos mesmos.
  - Nesse projeto fazemos uso do JUnit 5, o que nos da a possibilidade de usar a anotação DisplayName para dar descrições em Português para nossos testes.