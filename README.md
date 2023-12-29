# Projeto de Portfólio em Angular + .NET

## Introdução

Bem-vindo ao meu projeto de portfólio! Este é um projeto fullstack desenvolvido utilizando Angular para o frontend, .NET para os serviços de backend, e uma arquitetura de microservices para modularizar a aplicação. A utilização de contêineres facilita a execução do projeto em qualquer ambiente compatível.

Destaco que este portfólio vai além da apresentação estática de informações, permitindo aos usuários conectar diretamente com seu perfil do LinkedIn para exibir informações atualizadas e relevantes. Isso é possível graças à obtenção direta dos dados do Linkedin, sendo apenas necessário que o usuário passe um accessToken e profileName para o devido endpoint.

## Arquitetura do Projeto

### Frontend (Angular)

O frontend é desenvolvido em Angular, uma SPA (Single-Page Application) que proporciona uma experiência de usuário moderna e responsiva. A estrutura modular do Angular facilita a manutenção e escalabilidade do código.

### Backend Microservices (.NET)

O backend é implementado como microservices utilizando a tecnologia .NET 8. Cada microserviço é responsável por uma funcionalidade específica, seguindo os princípios de uma arquitetura distribuída. Os serviços incluem:

1. **Serviço do Portfólio:** Lida com a obtenção e atualização dos dados do portfólio.

### API Gateway (Nginx)

O API Gateway é construído utilizando Nginx, funcionando como um ponto de entrada para as requisições. Ele gerencia o roteamento das solicitações para os microservices apropriados e proporciona uma camada adicional de segurança.

### Conteinerização (Docker)

Todo o projeto é conteinerizado usando Docker, o que simplifica a implantação e garante a consistência entre os ambientes de desenvolvimento e produção.

## Instruções de Uso

1. **Configuração do Ambiente:**
   - Certifique-se de ter o Docker instalado em sua máquina.
   - Clone este repositório.

2. **Execução do Projeto:**
   - Navegue até o diretório raiz do projeto.
   - Execute `docker-compose up` para iniciar os contêineres.

3. **Acesso ao Portfólio:**
   - O frontend estará acessível em [http://localhost:4200](http://localhost:4200).
   - O API Gateway estará disponível em [http://localhost:8080](http://localhost:8080).

## Integração com LinkedIn

Este projeto permite a integração direta com o perfil do LinkedIn do usuário para exibição de informações atualizadas. Para habilitar esta funcionalidade, siga estes passos:

1. Faça login no seu perfil do LinkedIn.
2. Vá para [LinkedIn Developer Console](https://www.linkedin.com/developers/) e crie um aplicativo.
3. Copie as chaves de autenticação geradas para o arquivo de configuração apropriado.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para criar issues, enviar pull requests ou fornecer feedback.

Obrigado por explorar meu projeto de portfólio!
