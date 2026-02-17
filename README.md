# chatting-application
This is a project that uses Java as the core language to develop the frontend for a Chatting application for universities and Organizations.

Features
Real-Time Messaging:

Users can send and receive messages instantly.
Messages are broadcasted to all connected clients in a group chat setup.
End-to-end encryption:

The messages will be encrypted in the sender's side to be decrypted after recieving.
User-Friendly GUI:

Built using Java Swing, the application offers an easy-to-navigate interface for users.
Extensibility:

The modular design allows developers to easily add features like private messaging, message encryption, or multimedia support.
Getting Started
Prerequisites
Java Development Kit (JDK) version 11 or above
An IDE such as Visual Studio Code, IntelliJ IDEA, Eclipse, or NetBeans (optional)
PostgreSQL database installed on your system
Installation
Clone the repository:

git clone https://github.com/sahithdotk/ChattingAPP
Navigate to the project directory:

cd Chatting_Application
Compile the source code:

javac Chatting_Application/src/*.java
Set up the PostgreSQL database:

Install PostgreSQL if not already installed:
sudo apt update
sudo apt install postgresql postgresql-contrib
Start the PostgreSQL service:
sudo service postgresql start
Log in to the PostgreSQL shell:
sudo -u postgres psql
Create a new database and table:
CREATE DATABASE chatapp;
\c chatapp
CREATE TABLE chat_logs (
    id SERIAL PRIMARY KEY,
    sender VARCHAR(50),
    content TEXT,
    timestamp TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
Run the server:

java src/chatting/application/UserA.java
Run the client:

java src/chatting/application/UserB.java
To display the logged chats in pgAdmin's Query tool:

SELECt * FROM chat_Logs;
Contributions
Contributions are welcome! If you'd like to add features, improve the code, or fix bugs, feel free to fork the repository and submit a pull request.

License
This project is licensed under the MIT License.
