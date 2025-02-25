# RAG-based AI Chatbot using SpringBoot

## Overview
This project is an AI-powered chatbot built using the **Spring AI-SpringBoot** platform. The chatbot enables users to interact with PDF documents efficiently by leveraging **Retrieval-Augmented Generation (RAG)**. The chatbot extracts relevant information from PDFs and generates intelligent responses based on user queries.

## Features
- **PDF File Processing:** Reads and processes PDF documents for querying.
- **RAG-based Response Generation:** Enhances AI-generated responses with retrieved knowledge from PDFs.
- **Spring AI Integration:** Utilizes SpringBoot and Spring AI to handle queries and responses effectively.
- **Vector Database Support:** Uses embedding-based retrieval mechanisms to fetch relevant document content.
- **REST API Support:** Exposes API endpoints for easy integration with other applications.

## Technologies Used
- **SpringBoot** - Java-based framework for building microservices.
- **Spring AI** - AI framework to integrate large language models with Spring applications.
- **Apache PDFBox** - Library for reading and extracting text from PDF files.
- **OpenAI API** - (or any LLM provider) for intelligent response generation.
- **Pinecone / FAISS** - Vector database for document retrieval.
- **Maven** - Dependency management and build automation.

## Installation & Setup
### Prerequisites
Ensure you have the following installed:
- Java 17 or later
- Maven 3.x
- OpenAI API Key (or equivalent LLM provider key)

### Steps to Run
1. Clone the repository:
   ```sh
   git clone https://github.com/ak4721269/Rag-based-AI-chatbot-using-springboot.git
   ```
2. Navigate to the project directory:
   ```sh
   cd RAG-application
   ```
3. Build the project using Maven:
   ```sh
   mvn clean install
   ```
4. Configure environment variables:
   ```sh
   export OPENAI_API_KEY=your-api-key
   ```
5. Run the SpringBoot application:
   ```sh
   mvn spring-boot:run
   ```

## API Endpoints
### Upload PDF
```http
POST /api/pdf/upload
```
- **Description:** Uploads a PDF file for processing.
- **Request:** Multipart file upload.
- **Response:** JSON object with file metadata.

### Ask a Question
```http
POST /api/chat/query
```
- **Description:** Submits a query related to the uploaded PDF.
- **Request:** JSON body with query text.
- **Response:** AI-generated response based on document context.

## Code Structure
```
RAG application
│── src
│   ├── main
│   │   ├── java/com/soturit/musashi
│   │   │   ├── controllers (API Controllers)
│   │   │   ├── services (Business Logic)
│   │   │   ├── utils (Helper Classes)
│   │   │   ├── PdfFileReader.java (Handles PDF processing)
│   ├── resources
│       ├── application.properties (Configuration)
│── pom.xml (Maven Dependencies)
```

## Contribution
Contributions are welcome! Feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License.

## Contact
For any questions or issues, please contact me-ak4721269.

