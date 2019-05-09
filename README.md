# Projeto de criação de lista de convidados usando Spring Boot
Front-end e Back-end criados para sistema de geração de lista de convidados de evento com envio de email usando Spring Boot.

### Tecnologias/Ferramentas utilizadas:

* JDK 1.8.0_201
* Eclipse Version: 2019-03 (4.11.0)
* Apache Maven
* Jetty
* Thymeleaf
* SonarLint 4.1
* Checkstyle 8.18.0
* Actuator
* MySQL Community Server
* S.O. Windows

### Banco de Dados:
1. É preciso ter o MySQL Server rodando com o schema *listavip* criado.
2. Alterar o usuário e senha do banco no arquivo **application.properties** do projeto .

### Geração do fat jar em ambiente de desenvolvimento usando Eclipse:

* Clonar o projeto:

```sh
$ git clone https://git@github.com:americanolinhares/spring-boot-convidados.git
$ cd spring-boot-convidados
```

1. Dentro do Eclipse com a perspectiva **Java EE** ir em *File*->*Import*->*Maven*->*Existing Maven Projects*->*Next*;
2. Em *Root Directory* selecionar a pasta com o projeto baixado e depois *Finish*;
3. Clicar com o botão direito na pasta do projeto->*Run as*->*Maven Clean*;
4. Clicar com o botão direito na pasta do projeto->*Run as*->*Maven Install*;
5. Na pasta target do projeto será gerado o arquivo **listavip-1.0-SNAPSHOT.jar**.

### Execução da aplicação via linha de comandos:

1. Via terminal acessar a pasta onde o arquivo **listavip-1.0-SNAPSHOT.jar** acima foi gerado.
2. Executar o comando:

```
$ java -jar listavip-1.0-SNAPSHOT.jar
```

3. Através de um navegador acessar: http://localhost:9000.

### Dependência:

1. Para a funcionalidade de envio de email o projeto depende do jar **enviadorEmail-1.0-SNAPSHOT.jar** gerado pelo projeto [spring-boot-email](https://github.com/americanolinhares/spring-boot-email) encontrado no github: