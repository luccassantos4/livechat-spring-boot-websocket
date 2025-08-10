[JAVA_BADGE]: https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white
[SPRING_BADGE]: https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white
[AWS_BADGE]: https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white

<h1 align="center">Live Chat Spring Boot com WebSocket 💬</h1>

<p align="center">
  <img src="https://github.com/luccassantos4/livechat-spring-boot-websocket/blob/main/live-chat-print2.png?raw=true" width="600" alt="Live Chat Screenshot"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/java-21-blue?style=for-the-badge&logo=openjdk"/>
  <img src="https://img.shields.io/badge/spring-3.https://github.com/luccassantos4/livechat-spring-boot-websocket.git3.5-brightgreen?style=for-the-badge&logo=spring"/>
  <img src="https://img.shields.io/badge/websocket-STOMP-blueviolet?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/AWS-ElasticBeanstalk-orange?style=for-the-badge&logo=amazon-aws"/>
</p>

<p align="center">
  <b>Projeto de Live Chat em tempo real utilizando Spring Boot, WebSocket (STOMP) e hospedagem na AWS Elastic Beanstalk.</b>
</p>

---

## 📚 Sobre o Projeto

Este projeto é uma aplicação de chat em tempo real desenvolvida com Spring Boot e WebSocket (STOMP), permitindo a comunicação instantânea entre múltiplos usuários. A interface web é moderna e responsiva, construída com HTML, CSS e JavaScript, e o backend é preparado para fácil deploy em ambientes cloud como AWS Elastic Beanstalk.

### Principais Funcionalidades
- Envio e recebimento de mensagens em tempo real
- Interface web responsiva e intuitiva
- Comunicação via WebSocket utilizando STOMP
- Backend em Java 21 com Spring Boot 3.3.5
- Pronto para deploy em AWS Elastic Beanstalk

---

## 🛠️ Tecnologias Utilizadas
- **Java 21**
- **Spring Boot 3.3.5**
- **Spring WebSocket & STOMP**
- **HTML5, CSS3 (custom + Bootstrap), JavaScript (jQuery, STOMP.js)**
- **Maven**
- **AWS Elastic Beanstalk**

---

## 🚀 Como Executar Localmente

### Pré-requisitos
- [Java 21+](https://adoptium.net/)
- [Maven](https://maven.apache.org/)

### Clonando o repositório
```bash
 git clone https://github.com/luccassantos4/livechat-spring-boot-websocket.git
 cd livechat-spring-boot-websocket
```

### Configuração de Ambiente
No arquivo `src/main/resources/application.properties`:
```properties
server.port=5000 # ou defina a porta desejada
```

### Rodando o projeto
```bash
mvn spring-boot:run
```
Acesse: [http://localhost:5000](http://localhost:5000)

---

## 🖥️ Estrutura do Projeto
```
livechat-spring-boot-websocket/
├── src/
│   ├── main/
│   │   ├── java/luccassantos4/livechatms/
│   │   │   ├── LivechatmsApplication.java
│   │   │   ├── config/WebSocketConfig.java
│   │   │   └── controller/
│   │   │       ├── LiveChatController.java
│   │   │       ├── ChatInput.java
│   │   │       └── ChatOutput.java
│   │   └── resources/
│   │       ├── application.properties
│   │       └── static/
│   │           ├── index.html
│   │           ├── app.js
│   │           └── main.css
│   └── test/
│       └── java/luccassantos4/livechatms/LivechatmsApplicationTests.java
├── pom.xml
└── README.md
```

---

## ⚙️ Principais Componentes

### Backend (Java/Spring Boot)
- **LivechatmsApplication.java**: Classe principal da aplicação.
- **WebSocketConfig.java**: Configuração do endpoint WebSocket e do broker STOMP.
- **LiveChatController.java**: Controlador responsável por receber e enviar mensagens via WebSocket.
- **ChatInput.java / ChatOutput.java**: Records para modelar as mensagens de entrada e saída.

### Frontend (HTML/JS/CSS)
- **index.html**: Interface do chat.
- **app.js**: Lógica de conexão, envio e recebimento de mensagens via STOMP/WebSocket.
- **main.css**: Estilização customizada e responsiva.

---

## ☁️ Deploy na AWS Elastic Beanstalk

1. Gere o arquivo `.jar` com:
   ```bash
   mvn clean package
   ```
2. Faça upload do `.jar` gerado para o ambiente Elastic Beanstalk.
3. Configure as variáveis de ambiente necessárias (ex: `SERVER_PORT`).
4. Acesse a URL fornecida pela AWS para utilizar o chat em produção.

---