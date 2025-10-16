# RealTimeChat

A real-time chat application built with Spring Boot and WebSocket technology.

## Features

- Real-time messaging using WebSocket
- Bootstrap-based responsive UI
- SockJS for WebSocket fallback support
- Spring Boot backend with STOMP messaging protocol
- Input validation and error handling

## Technologies Used

- **Backend:** Spring Boot 3.3.5, WebSocket, STOMP
- **Frontend:** HTML5, Bootstrap 5, JavaScript, SockJS
- **Build Tool:** Maven
- **Java Version:** 17

## Getting Started

### Prerequisites

- Java 17 or higher
- Maven 3.6 or higher

### Running the Application

1. Clone the repository:
```bash
git clone https://github.com/ShivamSinghYadav25/RealTimeChat.git
cd RealTimeChat/chat-app
```

2. Run the application:
```bash
mvn spring-boot:run
```

3. Open your browser and navigate to:
```
http://localhost:8080/chat
```

## How to Use

1. Enter your name in the "Your name" field
2. Type your message in the message input field
3. Click "Send" to send the message
4. Messages will appear in real-time for all connected users

## Project Structure

```
chat-app/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/chat/app/
│   │   │       ├── AppApplication.java
│   │   │       ├── config/WebSocketConfig.java
│   │   │       ├── controller/ChatController.java
│   │   │       └── model/ChatMessage.java
│   │   └── resources/
│   │       ├── application.properties
│   │       └── templates/chat.html
│   └── test/
└── pom.xml
```

## API Endpoints

- `GET /chat` - Serves the chat interface
- `WebSocket /chat` - WebSocket endpoint for real-time communication
- `Message Mapping /app/sendMessage` - Handles message sending
- `Topic /topic/messages` - Broadcasts messages to all connected clients

## Contributing

Feel free to contribute to this project by submitting issues or pull requests.

## License

This project is open source and available under the [MIT License](LICENSE).