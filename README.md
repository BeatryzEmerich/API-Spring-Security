# Dio Spring Security

<img src="https://hermes.dio.me/articles/cover/d4bca4a7-c2ee-44b0-ac2f-2ecc0d1a1ac2.png" alt="Spring Security" />

## Descrição

O projeto Dio Spring Security é uma API Web desenvolvida com o Spring Boot que demonstra a implementação de segurança com o Spring Security. Ele fornece funcionalidades de autenticação e autorização, permitindo o controle de acesso a recursos protegidos com base em funções de usuário, vale ressaltar que foi desenvolvido com intuito de estudo.

## Tecnologias Utilizadas

- Spring Boot
- Spring Security
- Spring Data JPA
- H2 Database

## Configuração

Para executar este projeto em sua máquina local, siga estas etapas:

1. Clone o repositório para o seu ambiente local.
2. Certifique-se de que você tenha o Java JDK 17 instalado.
3. Configure as propriedades do banco de dados H2 no arquivo `application.properties` se necessário.
4. Execute a aplicação Spring Boot usando a IDE de sua escolha ou o comando `./mvnw spring-boot:run`.
5. Acesse a API em `http://localhost:8080`.
6. Certifique das versões das suas dependencias 

## Funcionalidades Principais

- **Autenticação**: A API permite que os usuários façam login com suas credenciais (nome de usuário e senha).

- **Autorização**: Os endpoints da API são protegidos com base nas funções de usuário. Os usuários podem ter funções de "MANAGERS" e "USERS", e o acesso a recursos específicos é controlado com base nessas funções.

## Endpoints de Exemplo

- `/login` (POST): Permite que os usuários façam login e autentiquem-se no sistema.
- `/managers` (GET): Apenas os usuários com a função "MANAGERS" podem acessar este endpoint.
- `/users` (GET): Tanto os usuários com a função "USERS" quanto os "MANAGERS" podem acessar este endpoint.

## Segurança

A segurança é implementada com o uso do Spring Security. Certifique-se de configurar corretamente as funções de usuário e as permissões em seu projeto.

