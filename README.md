# 🤖 AI-Based Resume Generator

An intelligent resume generation application that uses OpenAI's GPT models to create professional, ATS-friendly resumes from user descriptions. Built with React and Spring Boot.

## 🌐 Live Demo

- **Frontend**: [https://ai-resume-generator-frontend-omega.vercel.app](https://ai-resume-generator-frontend-omega.vercel.app)
- **Backend API**: [https://ai-resume-generator-backend-lr6d.onrender.com](https://ai-resume-generator-backend-lr6d.onrender.com)

## ✨ Features

- 🎨 **AI-Powered Generation**: Leverages OpenAI GPT models to create tailored resumes
- 📝 **Smart Parsing**: Extracts key information from natural language descriptions
- 🎯 **Professional Templates**: Generates well-structured, ATS-friendly resume formats
- 💾 **Export Options**: Download resumes as PDF or images
- 📱 **Responsive Design**: Works seamlessly on desktop and mobile devices
- ⚡ **Real-time Preview**: See your resume as it's being generated
- 🔒 **Secure**: Environment-based API key management

## 🏗️ Architecture

### Frontend
- **Framework**: React 18 with Vite
- **Styling**: Tailwind CSS
- **Routing**: React Router
- **HTTP Client**: Axios
- **State Management**: React Hooks
- **UI Components**: React Hot Toast, React Icons
- **Export**: HTML-to-Image, React-to-Print

### Backend
- **Framework**: Spring Boot 3.4.2
- **Java Version**: 21
- **AI Integration**: Spring AI with OpenAI
- **Build Tool**: Maven
- **API**: RESTful endpoints

## 📁 Project Structure

```
AI Based Resume Generator/
├── ai_resume_generator_frontend/     # React frontend
│   ├── src/
│   │   ├── components/              # Reusable UI components
│   │   ├── pages/                   # Page components
│   │   ├── api/                     # API service layer
│   │   └── assets/                  # Static assets
│   ├── public/                      # Public assets
│   └── package.json
│
├── AI-Resume_Generator_Backend/      # Spring Boot backend
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/resume/backend/
│   │   │   │   ├── controller/     # REST controllers
│   │   │   │   ├── service/        # Business logic
│   │   │   │   ├── ResumeRequest.java
│   │   │   │   └── ResumeAiBackendApplication.java
│   │   │   └── resources/
│   │   │       ├── application.properties
│   │   │       └── resume_prompt.txt
│   │   └── test/                    # Unit tests
│   ├── Dockerfile
│   └── pom.xml
│
└── API_KEY.txt                       # API key reference (not committed)
```

## 🚀 Getting Started

### Prerequisites

- **Frontend**: Node.js 18+ and npm
- **Backend**: Java 21+ and Maven 3.9+
- **API Key**: OpenAI API key

### Frontend Setup

1. Navigate to the frontend directory:
```bash
cd ai_resume_generator_frontend
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file:
```env
VITE_API_BASE_URL=http://localhost:8080
```

4. Run the development server:
```bash
npm run dev
```

The frontend will be available at `http://localhost:5173`

### Backend Setup

1. Navigate to the backend directory:
```bash
cd AI-Resume_Generator_Backend
```

2. Create environment variables or update `application.properties`:
```properties
spring.ai.openai.api-key=${OPENAI_API_KEY}
spring.ai.openai.chat.options.model=${OPENAI_CHAT_MODEL:gpt-4o-mini}
```

3. Run the application:
```bash
./mvnw spring-boot:run
```

Or build and run the JAR:
```bash
./mvnw clean package
java -jar target/resume-ai-backend-0.0.1-SNAPSHOT.jar
```

The backend will be available at `http://localhost:8080`

## 🐳 Docker Deployment

### Build the Docker image:
```bash
cd AI-Resume_Generator_Backend
docker build -t ai-resume-backend .
```

### Run the container:
```bash
docker run -p 8080:8080 \
  -e OPENAI_API_KEY=your_api_key \
  -e OPENAI_CHAT_MODEL=gpt-4o-mini \
  ai-resume-backend
```

## ☁️ Cloud Deployment

### Frontend (Vercel)

1. Connect your GitHub repository to Vercel
2. Set the root directory to `ai_resume_generator_frontend`
3. Configure environment variable:
   - `VITE_API_BASE_URL`: Your Render backend URL
4. Deploy

### Backend (Render)

1. Create a new Web Service on Render
2. Connect your GitHub repository
3. Set the root directory to `AI-Resume_Generator_Backend`
4. Configure environment variables:
   - `OPENAI_API_KEY`: Your OpenAI API key
   - `OPENAI_CHAT_MODEL`: `gpt-4o-mini` (or preferred model)
5. Build command: `mvn clean package -DskipTests`
6. Start command: `java -jar target/resume-ai-backend-0.0.1-SNAPSHOT.jar`
7. Deploy

## 📡 API Endpoints

### Generate Resume
```http
POST /api/v1/resume/generate
Content-Type: application/json

{
  "userDescription": "Your resume description here"
}
```

**Response:**
```json
{
  "think": "AI reasoning process",
  "data": {
    "personalInfo": {...},
    "summary": "...",
    "experience": [...],
    "education": [...],
    "skills": {...},
    "projects": [...],
    "certifications": [...],
    "languages": [...]
  }
}
```

## 🛠️ Technologies Used

### Frontend
- React 18.3
- Vite 6.0
- Tailwind CSS 3.4
- Axios 1.7
- React Router 7.1
- React Hook Form 7.54
- React Hot Toast 2.5
- React Icons 5.4

### Backend
- Spring Boot 3.4.2
- Spring AI 1.0.0-M5
- OpenAI Spring Boot Starter
- Java 21
- Maven 3.9
- Jackson (JSON Processing)

## 🔧 Configuration

### Environment Variables

**Frontend (.env)**
```env
VITE_API_BASE_URL=http://localhost:8080
```

**Backend (Render/Docker)**
```env
OPENAI_API_KEY=sk-your-api-key
OPENAI_CHAT_MODEL=gpt-4o-mini
```

## 🧪 Testing

### Frontend
```bash
npm run lint
```

### Backend
```bash
./mvnw test
```

## 📝 How It Works

1. **User Input**: User provides a natural language description of their background, skills, and experience
2. **API Request**: Frontend sends the description to the backend via REST API
3. **AI Processing**: Backend uses OpenAI's GPT model with a custom prompt template to generate structured resume data
4. **Response Parsing**: Backend parses the AI response into JSON format with sections like personal info, experience, education, etc.
5. **Display**: Frontend renders the structured data in a professional resume template
6. **Export**: User can download the resume as PDF or image

## 🐛 Troubleshooting

### Common Issues

**500 Internal Server Error**
- Ensure `resume_prompt.txt` exists in `src/main/resources/`
- Verify environment variables are set correctly in Render
- Check that OpenAI API key is valid and has sufficient credits
- Review Render logs for specific error messages

**CORS Errors**
- Verify frontend URL is in the `@CrossOrigin` annotation
- Check that backend is deployed and accessible

**Build Failures**
- Ensure Java 21 is being used
- Clear Maven cache: `./mvnw clean`
- Check internet connection for dependency downloads

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the MIT License.

## 👥 Authors

Built with ❤️ by the development team

## 🙏 Acknowledgments

- OpenAI for providing the GPT API
- Spring AI team for the excellent integration
- Vercel and Render for hosting services

---

**Note**: Make sure to never commit your `API_KEY.txt` or `.env` files containing sensitive information to version control.
