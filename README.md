# ChatVerse 💬

A full-stack real-time chat application built with Spring Boot and React, featuring WebSocket-based messaging, user authentication, and modern UI/UX design.

---

## 🔗 Live Deployment

- **Frontend**: [https://chat-verse-frontend-seven.vercel.app](https://chat-verse-frontend-seven.vercel.app)
- **Backend API**: [https://chat-verse-backend-zjzc.onrender.com](https://chat-verse-backend-zjzc.onrender.com)

---

## 📋 Project Demo

### 📹 Video Demonstration
Watch the complete walkthrough of E-Notes application:


<div align="center">
  <h3>
    <a href="https://drive.google.com/file/d/1ZAPUMzwsF9O_rPivvqOeEx4VcOHCRZVk/view?usp=drive_link">
      🎥 Watch Full Demo Video →
    </a>
  </h3>
  <p><em>Complete walkthrough of all features and functionalities</em></p>
</div>

*Video embedded from Google Drive - click play to watch*

### 📸 Application Screenshots

#### 🏠 Landing Page
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/472a39fd-a68b-47ee-a58e-53aa0b63e85c" />
*The home page welcomes users with a clean, modern interface showcasing the application's key features, hero section with call-to-action, and user testimonials.*

#### 🤖 AI Prompt Input
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/1ec8bf2e-3b32-4d4d-9896-a4f7dda366be" />
*Users can describe their experience and skills in natural language, and the AI will generate a professional resume automatically.*

#### 📝 Resume Form
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/a6e1c2a8-ed44-4cc3-8f46-55d0b9c4087b" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/b8d4f2c3-1955-48d1-a5ef-4bc9e1438e08" />
*For more control, users can manually fill in their information through a comprehensive form with sections for personal details, education, experience, and skills.*

#### 📄 Generated Resume
<img width="1916" height="1080" alt="Image" src="https://github.com/user-attachments/assets/ef820cf0-a837-4163-af38-7b04f9e12c8c" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/e2115526-0d64-4c31-ae13-0c0b5182fe88" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/2fea8394-31e3-4395-b6fc-e4ccdbf6d560" />
*The final professional, ATS-friendly resume with clean formatting, ready to download as PDF or image.*

---

## ✨ Features

- 🎨 **AI-Powered Generation**: Leverages OpenAI GPT models to create tailored resumes
- 📝 **Smart Parsing**: Extracts key information from natural language descriptions
- 🎯 **Professional Templates**: Generates well-structured, ATS-friendly resume formats
- 💾 **Export Options**: Download resumes as PDF or images
- 📱 **Responsive Design**: Works seamlessly on desktop and mobile devices
- ⚡ **Real-time Preview**: See your resume as it's being generated
- 🔒 **Secure**: Environment-based API key management

## 🎥 Demo Video

Watch a complete walkthrough of the AI Resume Generator in action:

https://github.com/user-attachments/assets/your-video-id-here

> **Note**: You can also find the demo video in the `screenshot` folder as `Project Video.mp4`. 
> 
> **To add the video to GitHub**: Upload the video to your GitHub repository's releases or use GitHub's drag-and-drop feature in the README editor to automatically host and embed the video.
>
> **Alternative**: If you want to host the video elsewhere, you can replace the link above with a YouTube, Vimeo, or Loom link.

## 📸 Screenshots & Pages

### Landing Page
The home page welcomes users with a clean, modern interface showcasing the application's key features and benefits.

**Features displayed:**
- Hero section with call-to-action button
- Feature cards highlighting AI-powered generation, multiple templates, and job-specific optimization
- User testimonials section
- Call-to-action footer

![Landing Page Screenshot](screenshot/1-Home.png)

---

### Generate Resume Page
This is the core functionality page where users can create their resume in two ways:

#### 1. AI Generation Mode (Prompt Input)
Users can describe their background in natural language, and the AI will automatically generate a structured resume.

**Key features:**
- Natural language text area for user description
- AI-powered generation button
- Clear/reset functionality
- Real-time loading indicators

![Generate Resume - AI Mode Screenshot](screenshot/2-Prompt.png)

**Example prompt:**
```
I am a software engineer with 5 years of experience in full-stack development. 
I have worked with React, Node.js, Spring Boot, and AWS. I graduated from MIT 
with a degree in Computer Science. I have led teams of 5 developers and delivered 
multiple successful projects.
```

#### 2. Form Edit Mode
After AI generation, users can review and manually edit all sections of their resume through an intuitive form interface.

**Editable sections include:**
- Personal Information (Name, Email, Phone, Location, LinkedIn, GitHub)
- Professional Summary
- Work Experience (Company, Position, Duration, Responsibilities)
- Education (Institution, Degree, Field, Year, GPA)
- Skills (Technical and soft skills)
- Projects (Title, Description, Technologies, Links)
- Certifications (Name, Issuer, Date)
- Languages (Language and proficiency level)
- Interests

**Form features:**
- Dynamic field arrays (add/remove multiple entries)
- Organized sections with clear labels
- Input validation
- Responsive layout

![Generate Resume - Form Mode Screenshot 1](screenshot/3-ResumeForm.png)

![Generate Resume - Form Mode Screenshot 2](screenshot/4-ResumeForm.png)

![Generate Resume - Form Mode Screenshot 3](screenshot/5-ResumeForm.png)

![Generate Resume - Form Mode Screenshot 4](screenshot/6-ResumeForm.png)

![Generate Resume - Form Mode Screenshot 5](screenshot/7-ResumeForm.png)

![Generate Resume - Form Mode Screenshot 6](screenshot/8-ResumeForm.png)

---

### Resume Preview & Export
Once the resume data is finalized, users can preview their professionally formatted resume and export it.

**Features:**
- Clean, ATS-friendly resume template
- Real-time preview of all sections
- **Export Options:**
  - Download as PDF (using React-to-Print)
  - Download as Image (using HTML-to-Image)
  - Print directly
- Responsive design for all screen sizes

**Resume sections displayed:**
- Header with contact information
- Professional summary
- Work experience with timeline
- Education background
- Technical skills grid
- Projects showcase
- Certifications
- Languages and interests

![Resume Preview Screenshot 1](screenshot/9-Resume.png)

![Resume Preview Screenshot 2](screenshot/10-Resume.png)

![Resume Preview Screenshot 3](screenshot/11-Resume.png)

---

### Navigation & Other Pages

#### About Page
Information about the application, its purpose, and the team behind it.

#### Services Page
Details about the services offered by the platform.

#### Contact Page
Contact form and information for user inquiries and support.

---

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

## 📝 How It Works - Step by Step Guide

### Step 1: Landing Page
When you first visit the application, you'll see a modern, welcoming interface that introduces you to the AI-powered resume generation features.

![Step 1 - Landing Page](screenshot/1-Home.png)

The landing page highlights:
- **Hero Section**: Clear call-to-action to get started
- **Key Features**: AI-powered generation, professional templates, and ATS optimization
- **User Benefits**: Quick resume creation with AI assistance

---

### Step 2: Enter Your Information (AI Prompt)
Click on "Generate Resume" to access the AI-powered input interface. Here, you simply describe your professional background in natural language.

![Step 2 - AI Prompt Input](screenshot/2-Prompt.png)

**What to include in your description:**
- Your current role and years of experience
- Technical skills and technologies you've worked with
- Educational background
- Notable projects or achievements
- Certifications or additional qualifications
- Career objectives or goals

The AI will understand your natural language description and automatically structure it into a professional resume format.

---

### Step 3: Review & Edit - Personal Information
After the AI generates your resume, you can review and edit every section. Start with your personal information:

![Step 3 - Personal Information Form](screenshot/3-ResumeForm.png)

**Editable fields:**
- Full Name
- Email Address
- Phone Number
- Location (City, State)
- LinkedIn Profile
- GitHub Profile
- Portfolio Website

---

### Step 4: Professional Summary & Experience
Refine your professional summary and work experience details:

![Step 4 - Summary and Experience](screenshot/4-ResumeForm.png)

**Work Experience Section:**
- Add multiple positions
- Company name and location
- Job title and employment dates
- Key responsibilities and achievements
- Use action verbs for impact

---

### Step 5: Education & Skills
Update your educational background and skill sets:

![Step 5 - Education and Skills](screenshot/5-ResumeForm.png)

**Education Details:**
- Institution name
- Degree type (Bachelor's, Master's, etc.)
- Field of study
- Graduation year
- GPA (optional)

**Skills Section:**
- Technical skills (programming languages, frameworks, tools)
- Soft skills (leadership, communication, problem-solving)
- Domain expertise

---

### Step 6: Projects & Certifications
Showcase your projects and professional certifications:

![Step 6 - Projects and Certifications](screenshot/6-ResumeForm.png)

**Projects:**
- Project title and description
- Technologies used
- Project links (GitHub, live demo)
- Your role and contributions

**Certifications:**
- Certification name
- Issuing organization
- Date obtained
- Validity period

---

### Step 7: Languages & Additional Information
Add language proficiencies and other relevant details:

![Step 7 - Languages and Interests](screenshot/7-ResumeForm.png)

**Languages:**
- Language name
- Proficiency level (Native, Fluent, Intermediate, Basic)

**Additional Sections:**
- Interests and hobbies
- Volunteer work
- Publications
- Awards and honors

---

### Step 8: Final Review
Complete the final review of all sections before generating the formatted resume:

![Step 8 - Final Form Review](screenshot/8-ResumeForm.png)

Make sure all information is:
- ✅ Accurate and up-to-date
- ✅ Free of typos and grammatical errors
- ✅ Formatted consistently
- ✅ Relevant to your target position

---

### Step 9: Resume Preview - Header & Summary
View your professionally formatted resume with a clean, ATS-friendly layout:

![Step 9 - Resume Preview Header](screenshot/9-Resume.png)

The preview shows:
- Professional header with contact information
- Well-formatted professional summary
- Clean typography and spacing
- ATS-optimized layout

---

### Step 10: Resume Preview - Experience & Education
Review your work experience and educational background in the formatted resume:

![Step 10 - Resume Experience Section](screenshot/10-Resume.png)

**Features:**
- Chronological work history
- Clear job titles and company names
- Bullet-pointed achievements
- Education section with relevant details
- Consistent formatting throughout

---

### Step 11: Export Your Resume
Finally, export your resume in your preferred format:

![Step 11 - Export Options](screenshot/11-Resume.png)

**Export Options:**
- 📄 **Download as PDF**: Perfect for email submissions and online applications
- 🖼️ **Download as Image**: Great for quick previews and social media
- 🖨️ **Print**: Direct printing with optimized layout

**Technical Process Behind the Scenes:**
1. **User Input**: Natural language description provided
2. **API Request**: Frontend sends data to Spring Boot backend via REST API
3. **AI Processing**: Backend uses OpenAI GPT model with custom prompt template
4. **Response Parsing**: AI response converted to structured JSON with all resume sections
5. **Display**: React components render the professional resume template
6. **Export**: HTML-to-Image and React-to-Print libraries handle the export functionality

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
