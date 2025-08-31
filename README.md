# vit-ap-pyq
<!-- PROJECT SHIELDS -->
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![TypeScript](https://img.shields.io/badge/language-TypeScript-blue.svg)]()
[![React](https://img.shields.io/badge/framework-React-61DAFB.svg)]()
[![Node.js](https://img.shields.io/badge/runtime-Node.js-339933.svg)]()
[![Express](https://img.shields.io/badge/framework-Express-000000.svg?style=flat&logo=express)]()
[![Next.js](https://img.shields.io/badge/framework-Next.js-000000.svg?style=flat&logo=next.js)]()
[![Tailwind CSS](https://img.shields.io/badge/style-Tailwind%20CSS-38B2AC.svg&logo=tailwindcss)]()


<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#description">Description</a></li>
    <li><a href="#features">Features</a></li>
    <li><a href="#tech-stack">Tech Stack</a></li>
    <li><a href="#installation">Installation</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#project-structure">Project Structure</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>



## Description
This project, named `vit-ap-pyq`, is a web application designed to provide AI-powered solutions for question papers. Users can upload question papers in various formats (PDF, PNG, JPG, TXT) or paste the questions directly into a text area. The application then uses OCR (Optical Character Recognition) and AI to extract the text and generate detailed, step-by-step solutions. It is built using a modern tech stack including React, TypeScript, Next.js, and Tailwind CSS for the frontend, and Node.js with Express for the backend. The backend leverages the Gemini AI model through the `@google/genai` library.



## ✨ Features
-   **File Upload**: Supports uploading question papers in PDF, PNG, JPG, and TXT formats.
-   **Text Input**: Allows users to directly paste question text.
-   **OCR Technology**: Uses Tesseract.js and sharp to extract text from images with high accuracy.
-   **AI-Powered Solutions**: Generates detailed, step-by-step solutions using the Gemini AI model.
-   **Secure API Handling**: API keys are stored securely using environment variables.
-   **Real-time Processing Status**: Provides feedback to the user regarding the status of the question paper processing.
-   **User Interface**: Modern, intuitive, and responsive user interface built with React and Tailwind CSS.
-   **Glassmorphism**: Utilizes glassmorphism effects to create a visually appealing UI.



## 💻 Tech Stack
-   **Frontend**:
    -   React
    -   TypeScript
    -   Next.js
    -   Tailwind CSS
    -   Radix UI
    -   React Hook Form
    -   Zod
    -   React Query

-   **Backend**:
    -   Node.js
    -   Express
    -   TypeScript
    -   @google/genai

-   **Database**:
    -   PostgreSQL (Neon)
    -   Drizzle ORM

-   **OCR**:
    -   Tesseract.js
    -   Sharp



## 🛠️ Installation
1.  **Clone the repository**:

    ```bash
    git clone https://github.com/Harshit052610/pyq-paradise.git
    cd pyq-paradise
    ```

2.  **Install dependencies**:

    ```bash
    npm install
    ```

3.  **Set up environment variables**:

    Create a `.env` file in the root directory and add your Gemini API key:

    ```
    GEMINI_API_KEY=YOUR_GEMINI_API_KEY
    DATABASE_URL=YOUR_DATABASE_URL
    ```

    Make sure to replace `YOUR_GEMINI_API_KEY` with your actual Gemini API key and `YOUR_DATABASE_URL` with your PostgreSQL database URL.

4.  **Database setup**:

    - Ensure that you have provisioned a PostgreSQL database. The project uses Neon.
    - Push the database schema using Drizzle Kit:

    ```bash
    npm run db:push
    ```



## 🚀 Usage
1.  **Start the development server**:

    ```bash
    npm run dev
    ```

2.  **Open the application in your browser**:

    Navigate to `http://localhost:5000` (or the port specified in your `.env` file).

3.  **Upload a question paper or paste text**:

    -   Click on the upload area and select a file (PDF, PNG, JPG, or TXT), or
    -   Paste the question text into the provided text area.

4.  **Generate Solutions**:

    -   Click the "Generate Solutions" button.

5.  **View and Export Solutions**:

    -   Once the processing is complete, the solutions will be displayed in a markdown format.
    -   You can copy the solutions to your clipboard or export them as a markdown file.



### Real-world use cases
1.  **Automated Question Paper Solving:**

    *   Teachers and educators can upload past exam papers to quickly generate model answers for student reference.

    *   Students can upload sample question papers to get detailed explanations and improve their understanding of concepts.

2.  **Textbook Problem Solutions:**

    *   Users can input problems from textbooks or study materials and obtain step-by-step solutions for self-assessment.

3.  **Quick Conceptual Understanding:**

    *   The application offers not just the answer but also explanations of the key concepts used, helping users grasp the underlying principles.

4.  **Homework Assistance:**

    *   Students can use it as a tool to verify their work, helping them understand the right approach and identify areas of improvement.



### Example Scenario
Imagine a student preparing for an upcoming physics exam. They have a sample question paper in PDF format but are unsure how to solve some of the problems.

1.  The student uploads the PDF file to the application.

2.  The OCR technology extracts the text from the PDF.

3.  The AI algorithms process the questions and generate step-by-step solutions, including explanations of the underlying physics concepts.

4.  The student reviews the solutions, understands the methodologies, and improves their problem-solving skills.



## 📂 Project Structure
```text
rest-express/
├── client/                  # React frontend
│   ├── src/                 # Frontend source code
│   ├── index.html           # HTML entrypoint
│   └── ...
├── server/                  # Node.js/Express backend
│   ├── index.ts             # Backend entrypoint
│   ├── routes.ts            # API routes
│   ├── services/          # Backend services (AI, OCR, etc.)
│   └── ...
├── shared/                  # Shared code between frontend and backend
│   ├── schema.ts            # Data schemas
│   └── ...
├── .env                     # Environment variables
├── package.json             # Project dependencies and scripts
├── tsconfig.json            # TypeScript configuration
└── README.md
```



## ✍️ Contributing
Contributions are always welcome!

1.  Fork the repository
2.  Create a new branch with descriptive name
3.  Commit your changes
4.  Push to the branch
5.  Open a pull request



## 📝 License
This project is licensed under the MIT License - see the [LICENSE](https://opensource.org/licenses/MIT) file for details.



## :link: Important links
*   **Repository**: [https://github.com/Harshit052610/pyq-paradise](https://github.com/Harshit052610/pyq-paradise)

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/Harshit052610">Harshit</a> and <a href="">Bhavesh</a>
</p>

<p align="center">
  <a href="https://github.com/Harshit052610/pyq-paradise"><b>Fork this project</b></a>
</p>

<p align="center">
  Give a ⭐ if this project helped you!
</p>
