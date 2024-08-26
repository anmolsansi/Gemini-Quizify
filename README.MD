# **Gemini-Quizify**

### **Overview**
Gemini-Quizify is an AI-powered quiz platform designed to provide students and learners with an interactive and personalized way to deepen their understanding of various subjects. Leveraging advanced AI technology, it generates dynamic quizzes from user-provided documents, such as textbooks and research papers. Users receive immediate feedback and detailed explanations, promoting better comprehension and retention of knowledge, ultimately enriching the overall learning experience.

This project utilizes technologies such as Google Gemini, Vertex AI API, Langchain, Google Service Accounts, PDF loaders, and Streamlit. Gemini-Quizify is part of the Radical AI challenge, with substantial contributions that push the boundaries of AI-driven educational tools.

---

### **Objective**
Learners often face challenges in reinforcing their understanding of complex topics due to limited access to effective study tools and immediate feedback. Gemini-Quizify addresses this problem by offering an AI-powered assessment and quiz tool designed to enhance learning through personalized quizzes, instant feedback, and comprehensive explanations. The goal is to build an intuitive platform that allows users to refine their skills, solidify their knowledge, and excel in their academic and professional pursuits.

---

### **Features**
- **AI-Generated Quizzes and Assessments**: Automatically creates quizzes from user-provided content, such as textbooks and academic papers, using AI-powered analysis.
- **Instant Feedback**: Provides immediate feedback on performance, helping users identify strengths and areas for improvement.
- **Comprehensive Explanations**: Each quiz question comes with detailed explanations, promoting better understanding of the material.
- **Tailored Learning Experience**: Quizzes are dynamically tailored to match the content provided by the user, ensuring relevance and alignment with their learning goals.

---

### **Technologies Used**
- **Python**: Powers the backend logic of Gemini-Quizify.
- **Langchain**: Provides natural language processing capabilities for analyzing and understanding textual content.
- **ChromaDB**: Manages storage and retrieval of user data and quiz content for efficient performance.
- **Google Gemini**: Enables AI-driven content analysis and dynamic quiz generation from user documents.
- **Streamlit**: Enhances user interaction through an intuitive web interface, allowing easy access to the quiz platform.

---

### **Setup Steps**
Follow these detailed steps to set up Gemini-Quizify:

#### 1. **Create a Google Cloud Account**
- Visit the [Google Cloud website](https://cloud.google.com/).
- Sign in with your Google account or sign up if you don’t have one.
- New users receive $300 in credits as part of the free trial.

#### 2. **Create a Google Cloud Project**
- Go to the [Google Cloud Console](https://console.cloud.google.com/).
- Select the project drop-down and click “New Project.”
- Enter your project details, choose a billing account, and click “Create.”

#### 3. **Enable Required APIs**
- Navigate to "APIs & Services" > "Library."
- Enable the following APIs:
  - AI Platform API
  - Google Gemini API (if applicable)
  - Other necessary APIs (e.g., Cloud Storage, Compute Engine).

#### 4. **Create a Service Account and Key**
- Go to "IAM & Admin" > "Service accounts."
- Create a new service account, granting necessary roles like AI Platform Admin and Google Gemini User.
- Generate a JSON key file for authentication and store it securely.

#### 5. **Set Up Your Project Directory**
- Create a `/secrets` directory in your project's root folder.
- Move the JSON key file to the `/secrets` directory for authentication.

---

### **Tasks Completed**
1. Integrated Google Service Account for secure authentication.
2. Developed a PDF loader for document ingestion.
3. Implemented Google Gemini for document processing and quiz generation.
4. Generated text embeddings using Langchain for accurate content representation.
5. Built a user-friendly interface with Streamlit.
6. Created dynamic quizzes based on user-specified topics.
7. Provided comprehensive explanations for quiz answers.
8. Implemented error handling and input validation for improved reliability.

---

### **Acknowledgments**
This project builds upon the foundation provided by the [mission-quizify](https://github.com/radicalxdev/mission-quizify) repository, developed by [radicalxdev]. We are grateful for their contributions.

Special thanks to:
- **[Radical AI](https://www.radicalai.org/)**: For inspiring the development of AI-driven learning tools.
- **[Streamlit](https://streamlit.io/)**: For simplifying the creation of interactive web applications.
- **[Google Cloud Platform](https://cloud.google.com/)**: For offering the APIs and services that power the core functionalities of this project.
- **[Langchain](https://langchain.com/)**: For enabling text embedding and AI-powered content analysis.

---