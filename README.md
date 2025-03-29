# 📧 Email Writer

## 📌 Overview
Email Writer is a web application that leverages the **Gemini API** to generate professional email responses based on user input. Built with **Spring Boot** for the backend and **React** for the frontend, this project provides a seamless user experience for generating AI-powered email replies.

## 🚀 Features
- 🤖 AI-powered email response generation using the **Gemini API**.
- 🌐 RESTful API with **Spring Boot**.
- 🎨 Modern and responsive UI built with **React**.
- 🔒 Secure API integration.
- 🎭 Supports different tones for generated emails.

## 🛠 Tech Stack
### Backend:
- ☕ Java
- 🏗 Spring Boot
- 🔗 WebClient for API calls

### Frontend:
- ⚛️ React
- ⚡ Vite
- 🎨 Material-UI
- 🌍 Axios

## 📥 Installation

### Prerequisites
Ensure you have the following installed:
- **☕ Java 17+**
- **🟢 Node.js** (latest LTS version recommended)
- **📦 Maven**

### Backend Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/Ajaykumar-058/email-writer.git
   ```
2. Navigate to the backend folder:
   ```sh
   cd email-writer/email-writer-api
   ```
3. Configure the application properties:
   ```properties
   spring.application.name=email-writer
   gemini.api.url=https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent
   gemini.api.key=YOUR_GEMINI_API_KEY
   ```
4. Build and run the backend:
   ```sh
   mvn spring-boot:run
   ```

### Frontend Setup
1. Navigate to the frontend folder:
   ```sh
   cd email-writer/email-writer-react
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the development server:
   ```sh
   npm run dev
   ```

## 📡 API Documentation
### 🔗 Endpoint: Generate Email Response
- **📍 URL:** `/api/email/generate`
- **📨 Method:** `POST`
- **📥 Request Body:**
  ```json
  {
    "emailContent": "Your original email content here",
    "tone": "polite"
  }
  ```
- **📤 Response:**
  ```json
  {
    "response": "Generated email reply here"
  }
  ```

## ⚠️ Troubleshooting
### 🛑 Common Issues
1. **Spring Boot Application Fails to Start**
   - ✅ Ensure you have configured `application.properties` correctly.
   - 🔑 Check if the API key is valid.

2. **Frontend Build Issues**
   - 📦 Run `npm install` to install missing dependencies.
   - 🎨 If **Material-UI** is missing, install it manually:
     ```sh
     npm install @mui/material @emotion/react @emotion/styled
     ```

## 🚀 Deployment
To deploy the application:
1. **Backend:**
   - 📦 Package the Spring Boot application:
     ```sh
     mvn package
     ```
   - ☁️ Deploy the generated JAR file to **Render** or any cloud provider.

2. **Frontend:**
   - 🏗 Build the React application:
     ```sh
     npm run build
     ```
   - 🚀 Deploy to **Vercel**, **Netlify**, or any hosting service.

## 🤝 Contribution Guidelines
We welcome contributions! To contribute:
1. 🔀 Fork the repository.
2. 🌱 Create a feature branch (`git checkout -b feature-branch-name`).
3. 📝 Commit changes (`git commit -m "Added new feature"`).
4. 📤 Push to the branch (`git push origin feature-branch-name`).
5. 🛠 Open a Pull Request.

## 📜 License
This project is licensed under the **MIT License**.

## 📩 Contact
For any inquiries, reach out via **GitHub Issues** or contact **Ajay Kumar**.

