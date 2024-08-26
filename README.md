# Gemini-Quizify

### Overview:
This AI-powered quiz platform is designed to provide students and learners with an interactive way to enhance their understanding of various subjects. By leveraging advanced AI, it generates quizzes from user-provided documents, offering immediate feedback and detailed explanations to support better comprehension and memory retention, ultimately enriching the learning experience.

The project implements this Quiz Builder using technologies like Google Gemini, Vertex AI API, embeddings, Google Service Account, Langchain, PDF loader, and Streamlit. It is part of challenges presented by Radical AI, where significant contributions have been made to implement specific steps, further pushing the boundaries of AI-driven learning tools.


### Objective:
Students and learners often struggle to reinforce their understanding of various subjects due to limited access to effective study tools and timely feedback. Addressing this challenge, the team is creating an AI-powered assessment and quiz tool designed to enhance learning by offering instant feedback and comprehensive explanations. This tool dynamically generates quizzes based on user-provided content, such as textbooks and research papers, delivering a personalized and engaging learning experience. The goal is to build a user-friendly platform that helps individuals refine their skills, deepen their knowledge, and excel in their academic endeavors.

### Features:
- **AI-Generated Assessments and Quizzes**: Leveraging AI, the tool generates quizzes and assessments dynamically from user-provided documents, including textbooks and scholarly papers.
- **Instant Feedback**: Users receive immediate feedback on their quiz performance, helping them quickly identify strengths and areas for improvement.
- **Comprehensive Explanations**: Each question is accompanied by detailed explanations, enabling users to grasp the reasoning behind correct answers and learn from their mistakes.
- **Tailored Learning Experience**: The quizzes are customized to the specific content provided by the user, ensuring relevance and alignment with the topics being studied.

### Technologies Used:
- **Python**: Forms the backbone of Gemini Quizify’s backend logic.
- **Langchain**: Powers the natural language processing capabilities, enabling the tool to analyze and understand textual content.
- **ChromaDB**: Manages data storage and retrieval, ensuring efficient handling of user data and quiz content.
- **Google Gemini**: Drives AI content analysis and generation, facilitating the dynamic creation of quizzes from user documents.
- **Streamlit**: Enhances user interaction by allowing the development of interactive web applications in Python, improving the accessibility and usability of Gemini Quizify.


### Setup Steps

Here are the detailed steps to set up your project, including creating a Google Cloud account, setting up a project, creating a service account with the required permissions, and organizing your project directory:

#### 1. Create a Google Cloud Account
- **Visit Google Cloud**: Go to the [Google Cloud website](https://cloud.google.com/).
- **Sign Up/In**: Click on the "Get started for free" button and sign in with your Google account or sign up if you don’t have one.
- **Free Trial**: New users receive $300 in credits during the free trial period.

#### 2. Create a Google Cloud Project
- **Go to Google Cloud Console**: Navigate to the [Google Cloud Console](https://console.cloud.google.com/).
- **Create a New Project**:
  - Click on the project drop-down menu at the top of the page.
  - Select “New Project.”
  - Enter your project name, select a billing account, and choose a location.
  - Click “Create.”

#### 3. Enable Required APIs
- **Navigate to APIs & Services**: In the left-hand menu, go to "APIs & Services" > "Library".
- **Enable APIs**:
  - Search for and enable the following APIs:
    - **AI Platform API**
    - **Google Gemini API** (if applicable)
    - Any other APIs your project requires (e.g., **Cloud Storage**, **Compute Engine**).

#### 4. Create a Service Account and Key
- **Navigate to IAM & Admin**: In the left-hand menu, go to "IAM & Admin" > "Service accounts".
- **Create a Service Account**:
  - Click “Create Service Account.”
  - Enter a name and description for the service account.
  - Click “Create and continue.”
- **Grant Permissions**:
  - In the "Grant this service account access to project" section, add the required roles:
    - **AI Platform Admin**
    - **Google Gemini User**
    - Add other roles as needed (e.g., **Storage Admin** for Cloud Storage).
  - Click "Continue."
- **Create a Key**:
  - Click “Done” to finish creating the service account.
  - In the service account list, select the newly created service account.
  - Go to the “Keys” tab.
  - Click "Add Key" > "Create new key."
  - Select "JSON" and click "Create."
  - Download the JSON key file (this is your service account key).

#### 5. Set Up Your Project Directory
- **Create a `/secrets` Directory**:
  - In the root folder of your project repository, create a directory named `secrets`.
- **Place the Service Account Key File**:
  - Move the downloaded JSON key file to the `/secrets` directory. This key will be used to authenticate your service account with Google Cloud.

You now have your project set up with the necessary Google Cloud resources and a structured project directory!


### Tasks Completed

The following tasks have been successfully integrated into the project:

1. **Google Service Account Integration**: Set up authentication using Google Service Account to securely access Google Cloud resources.
2. **PDF Loader Implementation**: Developed functionality for document ingestion, enabling users to upload and process PDFs.
3. **Processing Documents with Google Gemini**: Integrated Google Gemini for advanced content analysis and processing.
4. **Text Embedding Generation**: Utilized Langchain to generate text embeddings for efficient content representation and analysis.
5. **Streamlit User Interface**: Built an interactive user interface with Streamlit to enhance accessibility and user experience.
6. **Quiz Generation Based on User-Specified Topics**: Developed dynamic quiz generation that tailors questions to user-provided topics.
7. **Explanations for Quiz Answers**: Provided detailed explanations for each quiz answer, facilitating deeper learning and comprehension.
8. **Error Handling and Validation**: Implemented error handling and validation mechanisms to ensure robustness and reliability across different user inputs and scenarios.

### Acknowledgments

This project is built upon the foundation laid by the [mission-quizify](https://github.com/radicalxdev/mission-quizify) repository, originally developed by [radicalxdev]. We extend our gratitude to them for their excellent work.

Special thanks to the following organizations and tools for their contributions to this project:

- **[Radical AI](https://www.radicalai.org/)**: For inspiring and challenging us with their thought-provoking ideas.
- **[Streamlit](https://streamlit.io/)**: For providing a user-friendly platform for creating interactive interfaces.
- **[Google Cloud Platform](https://cloud.google.com/)**: For offering essential APIs and services that powered the core functionality of this project.
- **[Langchain](https://langchain.com/)**: For enabling text embedding generation and facilitating the AI-driven aspects of this project.



*********************************************************
Certainly! Here's an edited and refined version of the README file for your Gemini-Quizify project:

---

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