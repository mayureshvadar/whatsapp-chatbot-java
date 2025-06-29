# whatsapp-chatbot-java
This project is a Java-based WhatsApp chatbot built using Spring Boot and integrated with Firebase for message storage. It handles incoming messages via a webhook, auto-generates replies, and is deployable on Render for real-time interaction.

# 📱 WhatsApp Chatbot – Java + Spring Boot + Firebase

A fully functional WhatsApp chatbot backend built using **Java**, **Spring Boot**, and **Firebase Firestore**. This project demonstrates webhook handling, message auto-reply logic, cloud integration, and deployment on **Render** for a scalable real-world chatbot service.

---

## 🚀 Features

- Webhook endpoint (`/webhook`) for WhatsApp Cloud API
- Auto-reply logic based on message keywords
- Firestore integration for message logging
- Ngrok + Postman setup for local simulation
- Cloud deployment on Render

---

## 🧱 Tech Stack

- **Backend**: Java 17, Spring Boot
- **Database**: Firebase Firestore
- **Testing Tools**: Ngrok, Postman
- **Deployment**: Render
- **Build Tool**: Maven

---

## 💡 How It Was Built

- Initially developed using Java servlet to receive and parse incoming webhook payloads.
- Migrated to Spring Boot with clean REST controller architecture.
- Integrated Firebase Admin SDK to store messages and replies.
- Tested interactions using Ngrok tunnels and Postman with JSON mock payloads.
- Resolved typical issues like port conflicts, HTTP 3200 errors, and malformed headers.
- Connected the GitHub repo to Render and deployed a fully cloud-based chatbot backend.

---

## 📂 Project Structure


---

## 🔧 Running Locally

```bash
# Step 1: Clone and enter project
git clone https://github.com/your-username/whatsappbot.git
cd whatsappbot

# Step 2: Run the Spring Boot app
./mvnw spring-boot:run

# Step 3: Start ngrok to expose local server
ngrok http 8080

Test with Postman by sending a POST request to:
https://your-ngrok-url.ngrok.io/webhook


☁️ Deployment
- Deployed on Render
- Connected via GitHub and configured build/start commands
- Environment variables securely managed via Render dashboard

✅ Example Replies

Hi - Hey there! How can I assist you today?

Bye -Goodbye! Have a great day.

Anything else - You said: [user message]


📜 License & Credits
Developed by Mayureshvadar for a full-stack chatbot assignment demonstrating backend development, integration, and cloud deployment skills.

