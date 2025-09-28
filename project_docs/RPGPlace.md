# RPGPlace

RPGPlace é uma aplicação web completa para gerenciamento de mesas de RPG, permitindo que mestres e jogadores se conectem e joguem em tempo real.

## 1. Visão Geral do Projeto

O projeto é dividido em duas partes principais:

- **Backend:** Uma API RESTful desenvolvida em Java com Spring Boot, responsável pela lógica de negócio, gerenciamento de dados e autenticação.
- **Frontend:** Uma aplicação de página única (SPA) desenvolvida em Angular, que fornece a interface do usuário.

## 2. Tecnologias

### Backend

- **Java 21**
- **Spring Boot 3**
- **Spring Web, Data JPA, Security, WebSocket**
- **Maven**
- **PostgreSQL**
- **Docker**

### Frontend

- **Angular 20**
- **TypeScript**
- **RxJS**
- **Tailwind CSS**
- **StompJS e SockJS** (para WebSockets)

## 3. Como Executar o Projeto Completo

Para executar o projeto completo, você precisará ter o Java e Node.js instalados.

1. **Execute o Backend:**

   Navegue até o diretório `RPGPlaceJava` e siga as instruções no `README.md` do backend.

   ```bash
   cd RPGPlaceJava
   mvn spring-boot:run
   ```

2. **Execute o Frontend:**

   Navegue até o diretório `RPGPlaceAngular` e siga as instruções no `README.md` do frontend.

   ```bash
   cd RPGPlaceAngular
   npm install
   npm start
   ```

   A aplicação estará disponível em `http://localhost:4200`.

## 4. Estrutura do Repositório

- `RPGPlaceJava/`: Contém o código-fonte do backend.
- `RPGPlaceAngular/`: Contém o código-fonte do frontend.
- `RPGPlace.md`: Este arquivo, com a visão geral do projeto.

## 5. Contribuição

Contribuições são bem-vindas! Se você encontrar um bug ou tiver uma sugestão de melhoria, por favor, abra uma issue no repositório do GitHub. Se você quiser contribuir com código, por favor, crie um fork do repositório e envie um pull request.