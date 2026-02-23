# AI-Powered Code Reviewer

An **AI-powered full-stack web application** that provides instant, professional-level code reviews using **Google Gemini AI**.  
Built with the **MERN stack (Node.js, Express, React)**, this tool helps developers identify bugs, improve code quality, and follow best practices in real time.

---

## Features

- **AI-Driven Code Analysis**  
  Uses **Gemini 2.0 Flash** to analyze up to **10,000 lines of code** in a single request.

- **Real-Time Feedback**  
  Instantly detects:
  - Errors and bugs  
  - Code smells  
  - Performance issues  
  - Best-practice violations (with explanations)

- **Interactive Code Editor**  
  - Syntax highlighting  
  - Smooth editing experience  
  - Developer-friendly UI

- **Markdown-Based Review Output**  
  AI responses are displayed in a clean Markdown format with:
  - Highlighted code blocks  
  - Clearly separated issues and fixes

- **System-Tuned AI Behavior**  
  Custom system instructions ensure the AI behaves like an **experienced software engineer and code reviewer**.

---

## Tech Stack

### Frontend
- React (Vite)
- Axios
- PrismJS
- React Simple Code Editor
- React Markdown
- rehype-highlight

### Backend
- Node.js
- Express.js
- CORS
- Dotenv

### AI Integration
- Google Generative AI (`@google/generative-ai`)

---

## Prerequisites

Make sure you have the following installed:

- **Node.js**
- **Gemini API Key** from Google AI Studio

---

## Installation & Setup

### Backend Setup

1. Navigate to the backend folder:
   ```bash
      cd backend
   ```
2. Install dependencies:
   ```bash
     npm install express dotenv cors @google/generative-ai
   ```
3. Create a .env file in the backend root:
   ```bash
   GEMINI_API_KEY=your_api_key_here
   ```
4. Start the backend server:
   ```bash
   npx nodemon server.js
   ```
Server runs on http://localhost:3000

### Frontend Setup

1. Navigate to the frontend folder:
   ```bash
   cd frontend

2. Install dependencies:
   ```bash
    npm install axios prismjs react-simple-code-editor react-markdown rehype-highlight

3. Start the frontend development server:
   ```bash
   npm run dev

-**Then Paste code and click Review.**

###API Endpoints
 1. Test Server
    ```bash
    GET /
   
 2. AI Code Review
   POST /ai/get-review

 3. Request Body
   {
      "code": "your code here"
   }

 4. Response
  -Bug detection
  -Code improvement suggestions
  -Best-practice explanations
