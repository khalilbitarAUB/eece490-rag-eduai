# EduAI: An AI-Powered Knowledge Assistant for Educational Institutions

**Author:** Khalil Bitar  
**Affiliation:** Computer Science & Engineering Student, American University of Beirut (AUB)  
**Contact:** [kmb27@mail.aub.edu](mailto:kmb27@mail.aub.edu)

---

## 📖 Project Overview

Educational institutions generate extensive documentation including academic policies, research papers, syllabi, and administrative guidelines. Currently, students, faculty, and administrative staff face difficulties accessing relevant information quickly due to inefficient manual searching processes.

EduAI addresses this problem through an **AI-powered retrieval-augmented generation (RAG)** solution, providing accurate, document-based answers to queries posed by university students, faculty, and administrators.

---

## 🚀 Features

- **Document Ingestion and Indexing:** Supports PDFs, Word documents, research papers, policies, and FAQs.
- **Retrieval-Augmented Generation (RAG):** Provides conversational answers based on semantic search.
<!-- - **Integration Capabilities:** Seamlessly integrates with university portals, chatbots, and LMS platforms (e.g., Moodle, Blackboard). -->
- **Multi-Tenant Architecture:** Supports multiple institutions simultaneously.
<!-- - **Plug-and-Play API:** Simple integration into existing university systems. -->
<!-- - **Cloud & On-Premise Deployment:** Flexible deployment options respecting institutional security policies. -->

---

## 🛠️ Technical Implementation

EduAI is built upon a Retrieval-Augmented Generation (RAG) framework derived and customized from the open-source Kotaemon project [1].

### AI & ML Models
- **LLMs:** OpenAI GPT, AzureOpenAI, Claude, Google Gemini, Cohere Chat (Fine-tuned for contextual accuracy).
- **Semantic Search:** ChromaDB Vector Databases. Embeddings stored and retrieved using vector databases.

### RAG Pipeline
- Document ingestion and preprocessing.
- Embedding and semantic indexing of institutional content.
- Retrieval and ranking of relevant document snippets.
- Contextual answer generation using an optimized Large Language Model (LLM).

### Backend and Frontend Technologies
- **Backend:** FastAPI integrated with LangChain for document processing and API handling.
- **Frontend:** Gradio, providing interactive chat-based Q&A capabilities.

### Vector Database
- **ChromaDB:** For efficient semantic search and retrieval operations.

### Deployment
- Containerized using **Docker** to ensure portability and ease of deployment on cloud services such as AWS, GCP, or on-premises infrastructures.

---

## 📦 Technology Stack

| Component        | Technology                                    |
|------------------|-----------------------------------------------|
| **Framework**    | FastAPI, LangChain                            |
| **Frontend**     | Gradio                                        |
| **Vector DB**    | ChromaDB                                      |
| **AI Models**    | GPT, Gemini, Claude                           |
| **Containerization** | Docker                                    |

---

## 🎓 Reference & Citation

This project leverages and builds upon the open-source Kotaemon project:

```bibtex
@misc{kotaemon2024,
    title = {Kotaemon - An open-source RAG-based tool for chatting with any content.},
    author = {The Kotaemon Team},
    year = {2024},
    howpublished = {\url{https://github.com/Cinnamon/kotaemon}},
}


## 📚 Data Sources
EduAI utilizes various institutional data, including:

- University policies and academic guidelines
- Course syllabi, lecture materials, and grading criteria
- Student handbooks, administrative workflows, and FAQs

---

## 📈 Business Validation & Market Fit

### Why EduAI?
- Increasing adoption of AI-driven educational solutions.
- Demand for chatbot-based self-service solutions in higher education.
- Compliance with accreditation requirements for efficient document access.

### Target Users & Benefits
| Users                 | Benefits                                            |
|-----------------------|-----------------------------------------------------|
| **Students**          | Instant access to course info, policies, and research |
| **Faculty**           | Quick retrieval of institutional policies and research materials |
| **Administrative Staff** | Automation of repetitive queries regarding admissions, scholarships, etc. |

---

## 🌟 Competitive Edge & Scalability
- **Accurate, Document-Backed Answers:** Significantly reduces manual searches.
- **Instantaneous Responses:** Enhances decision-making speed.
- **Flexible Integration:** Multi-tenant architecture suitable for broad educational deployment.

---

## 📌 Future Expansion
- Integration with organizational tools (Slack, MS Teams, SharePoint, Google Drive).
- Processing multimedia content (images, videos, slides).
- Voice-based AI assistant for improved accessibility.
- Analytics dashboard to identify knowledge gaps and usage trends.
- Real-time document updates and user-role-based document access.
- Multilingual query and translation support.

---

## 🧪 MLOps & Documentation
The project follows best practices for Machine Learning Operations (MLOps), including clear documentation, Dockerization, and proper software methodology.

- **Dockerized Application**
- **Comprehensive API Documentation**
- **Detailed GitHub Repository**

---

## ✅ Quality Assurance & Testing
Extensive testing and validation procedures ensure the reliability, accuracy, and robustness of the EduAI solution.

---

## 📖 Repository Structure
```plaintext
EduAI
│
├── backend/           # Backend FastAPI and LangChain scripts
├── frontend/          # React frontend interface
├── models/            # AI models and embeddings
├── docs/              # Project documentation
├── Dockerfile         # Containerization configuration
├── requirements.txt   # Project dependencies
└── README.md          # Project overview and instructions
