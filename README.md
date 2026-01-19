\# AI-Powered Code Reviewer



A full-stack application that provides intelligent, real-time code reviews using Google's \*\*Gemini AI\*\*. The application features a sleek, split-pane interface where developers can write code and instantly receive feedback on potential bugs, optimization opportunities, and best practices.



\## 🚀 Features



\* \*\*AI-Driven Analysis:\*\* Leverages \*\*Gemini 2.0 Flash\*\* to analyze code logic, syntax, and style.

\* \*\*Interactive Editor:\*\* Built with `react-simple-code-editor` for a familiar coding experience.

\* \*\*Syntax Highlighting:\*\* Uses \*\*PrismJS\*\* for beautiful, readable code formatting.

\* \*\*Markdown Reports:\*\* Review results are rendered in rich Markdown (using `react-markdown`), making suggestions easy to read.

\* \*\*Clean UI:\*\* A modern, dark-themed interface with a responsive split-screen layout.



\## 🛠 Tech Stack



\*\*Frontend:\*\*

\* React (Vite)

\* PrismJS (Syntax Highlighting)

\* React Simple Code Editor

\* React Markdown \& Rehype Highlight

\* Axios



\*\*Backend:\*\*

\* Node.js

\* Express.js

\* Google Generative AI SDK (`@google/generative-ai`)

\* CORS



\## 📂 Project Structure



```text

├── backend/

│   ├── src/

│   │   ├── controllers/    # ai.controller.js (Handles AI requests)

│   │   ├── routes/         # ai.routes.js (API endpoints)

│   │   ├── services/       # ai.service.js (Gemini API config)

│   │   └── app.js          # Express setup

│   ├── server.js           # Entry point

│   └── .env                # API Keys

└── frontend/

&nbsp;   ├── src/

&nbsp;   │   ├── App.jsx         # Main UI (Split screen)

&nbsp;   │   └── App.css         # Custom styling

&nbsp;   └── vite.config.js



```



\## ✅ Prerequisites



\* Node.js installed.

\* A Google Cloud project with the \*\*Gemini API\*\* enabled.

\* An API Key from \[Google AI Studio](https://aistudio.google.com/).



\## ⚡ Installation \& Setup



\### 1. Backend Setup



Navigate to the backend directory and install dependencies:



```bash

cd backend

npm install



```



Create a `.env` file in the `backend` root:



```env

PORT=3000

GOOGLE\_GEMINI\_KEY=your\_gemini\_api\_key\_here



```



Start the server:



```bash

npm run dev

\# Server runs on http://localhost:3000



```



\### 2. Frontend Setup



Navigate to the frontend directory and install dependencies:



```bash

cd ../frontend

npm install



```



Start the Vite development server:



```bash

npm run dev

\# App runs on http://localhost:5173



```



\## 📖 Usage



1\. Open the web application.

2\. In the \*\*Left Panel\*\* (Code Editor), paste a snippet of code (e.g., a JavaScript function).

3\. Click the \*\*"Review"\*\* button.

4\. The application sends the code to the backend, which queries Gemini AI with a custom system prompt.

5\. The \*\*Right Panel\*\* displays a detailed review, including:

\* \*\*Issues Identification:\*\* Bugs or security risks.

\* \*\*Refactoring Suggestions:\*\* Cleaner or more efficient ways to write the code.

\* \*\*Corrected Code:\*\* A snippet showing the fixed version.







\## 🤝 Contributing



Contributions are welcome! Please fork the repo and submit a PR for any UI improvements or prompt engineering enhancements.



\## 📜 License



This project is licensed under the MIT License.

