# Industrial Knowledge Copilot

### ET AI Hackathon 2.0 – Phase 2 Build Sprint Submission

**Problem Statement 8:** AI for Industrial Knowledge Intelligence – Unified Asset & Operations Brain

**Team Name:** ParthPariwandh
**Team Lead:** Parth Pariwandh
**Institution:** Jadavpur University, Kolkata, India

---

## One AI Brain for Every Manual, Log and Lesson Your Plant Has Ever Written Down

Industrial organizations generate enormous amounts of operational knowledge through equipment manuals, maintenance records, inspection reports, standard operating procedures, safety documentation, quality records, audit findings, and engineering project files. Despite this abundance of information, critical knowledge often remains fragmented across multiple systems and departments, making it difficult to access when decisions need to be made.

Industrial Knowledge Copilot is an AI-powered Industrial Knowledge Intelligence Platform that transforms disconnected industrial documents into a unified, searchable, and actionable knowledge layer. By combining document intelligence, Retrieval Augmented Generation, knowledge graphs, compliance analysis, and maintenance insights, the platform enables engineers, operators, auditors, and managers to retrieve trustworthy answers with direct citations from source documents in seconds.

This project is developed as a submission for ET AI Hackathon 2.0 under the challenge theme of Industrial Knowledge Intelligence.

---

## Problem Statement

Asset-intensive industries frequently store information across multiple disconnected repositories.

Examples include:

* OEM Equipment Manuals
* Maintenance Logs
* Standard Operating Procedures
* Safety Documents
* Inspection Reports
* Regulatory Compliance Records
* Engineering Drawings
* Project Documentation

As a result:

* Engineers spend significant time searching for information.
* Critical operational knowledge remains siloed.
* Compliance verification becomes time-consuming.
* Failure patterns are often overlooked.
* Valuable expertise is lost when experienced personnel retire.

The challenge is to build a system capable of transforming these disconnected documents into a continuously accessible organizational knowledge asset.

---

## Proposed Solution

Industrial Knowledge Copilot provides a document-centric intelligence layer that enables users to:

* Upload industrial documents
* Extract engineering entities and relationships
* Build a lightweight industrial knowledge graph
* Search and retrieve information semantically
* Ask questions in natural language
* Receive source-cited answers
* Detect compliance gaps
* Discover maintenance patterns
* Preserve institutional knowledge

The platform focuses on practical deployment and rapid adoption while remaining technically robust and scalable.

---

## Key Features

### Universal Document Ingestion

Supports multiple document formats:

* PDF
* DOCX
* TXT
* Scanned Documents
* Images

Automatically processes uploaded documents for downstream analysis.

### OCR and Document Intelligence

Extracts:

* Text
* Tables
* Metadata
* Page References
* Section Information

Supports both digitally generated and scanned industrial documents.

### Knowledge Copilot

Engineers can ask questions such as:

* What is the lubrication interval for Pump P101?
* What maintenance activities were performed on Compressor A?
* Does this SOP satisfy lockout-tagout requirements?

The system responds with:

* Natural language answers
* Source references
* Page citations
* Confidence indicators

### Knowledge Graph

The platform builds a lightweight industrial knowledge graph linking:

* Equipment
* Parameters
* Personnel
* Documents
* Failures
* Regulations

This enables discovery of hidden relationships across documents.

### Compliance Intelligence

Automatically analyzes documents against:

* Factory Act
* OISD Guidelines
* PESO Requirements
* Internal Quality Systems

The platform identifies:

* Missing clauses
* Potential compliance gaps
* Audit concerns

### Maintenance Intelligence

Analyzes historical maintenance records to identify:

* Recurring failures
* Frequently affected equipment
* Emerging maintenance trends
* Potential root causes

### Dashboard and Analytics

Provides a centralized interface displaying:

* Uploaded documents
* Extracted entities
* Knowledge graph insights
* Compliance alerts
* Maintenance alerts
* User queries

---

## System Architecture

```text
Document Upload
       │
       ▼
OCR & Parsing Engine
       │
       ▼
Document Chunking
       │
       ▼
Entity Extraction
       │
       ▼
Knowledge Graph Generation
       │
       ▼
Embedding Generation
       │
       ▼
FAISS Vector Database
       │
       ▼
Retriever
       │
       ▼
Large Language Model
       │
       ▼
Answer Generation + Citations
       │
       ▼
Dashboard Interface
```

---

## Technology Stack

### Frontend

* Streamlit

### Backend

* FastAPI
* Python

### Document Processing

* PyMuPDF
* pdfplumber
* python-docx
* unstructured

### OCR

* Tesseract OCR
* EasyOCR

### NLP and Entity Extraction

* spaCy
* Sentence Transformers

### Retrieval Augmented Generation

* LangChain
* FAISS

### Knowledge Graph

* NetworkX

### Storage

* SQLite
* JSON

### Large Language Models

Supports interchangeable providers:

* Claude
* OpenAI
* OpenRouter-compatible models

---

## Repository Structure

```text
industrial-knowledge-copilot/

├── README.md
├── LICENSE
├── requirements.txt
├── .gitignore
├── .env.example

├── backend/
│   ├── app.py
│   ├── parser.py
│   ├── embeddings.py
│   ├── retriever.py
│   ├── knowledge_graph.py
│   └── compliance.py

├── frontend/
│   └── app.py

├── agents/
│   ├── maintenance_agent.py
│   ├── compliance_agent.py
│   └── copilot_agent.py

├── data/
│   └── sample_documents/

├── docs/
│   ├── architecture.png
│   ├── presentation.pdf
│   └── submission.pdf

├── prompts/

├── evaluation/

├── tests/

└── demo/
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/industrial-knowledge-copilot.git

cd industrial-knowledge-copilot
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

Windows:

```bash
venv\Scripts\activate
```

Linux/Mac:

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Running the Application

### Backend

```bash
uvicorn backend.app:app --reload
```

### Frontend

```bash
streamlit run frontend/app.py
```

---

## Demonstration Workflow

### Step 1

Upload industrial documents:

* Equipment Manual
* SOP
* Maintenance Logs
* Inspection Reports

### Step 2

Allow the system to:

* Parse documents
* Extract entities
* Build embeddings
* Generate knowledge graph

### Step 3

Ask technical questions.

Example:

```text
What is the lubrication interval for Pump P101?
```

### Step 4

Review the generated answer with source citations.

### Step 5

Open the Compliance Dashboard.

Review:

* Missing requirements
* Compliance observations

### Step 6

Open the Maintenance Dashboard.

Review:

* Failure patterns
* Maintenance insights
* Root cause indicators

---

## Business Impact

Industrial Knowledge Copilot delivers measurable value through:

### Faster Knowledge Retrieval

Reduces document search time from minutes to seconds.

### Better Compliance Readiness

Provides continuous visibility into potential compliance gaps.

### Improved Maintenance Planning

Surfaces recurring failures before they become major operational issues.

### Institutional Knowledge Retention

Preserves critical engineering knowledge in a searchable form.

### Improved Decision Support

Enables faster, evidence-backed engineering decisions.

---

## Future Scope

Future enhancements may include:

* Multi-language industrial document support
* Industrial ontology expansion
* Advanced graph analytics
* Integration with CMMS systems
* Integration with SCADA systems
* Mobile field technician application
* Predictive maintenance modules
* Digital twin integration
* Advanced regulatory intelligence

---

## Evaluation Metrics

The project is evaluated using:

* Entity Extraction Accuracy
* Retrieval Accuracy
* Citation Correctness
* Knowledge Graph Completeness
* Compliance Gap Detection Accuracy
* User Query Response Quality
* Time-to-Answer Improvement

---

## Team

### Team ParthPariwandh

**Team Lead**

Parth Pariwandh

Mechanical Engineering Undergraduate

Jadavpur University

Kolkata, India

---

## Acknowledgements

This project was developed as part of ET AI Hackathon 2.0.

The team acknowledges the open-source communities behind:

* FastAPI
* Streamlit
* LangChain
* FAISS
* spaCy
* NetworkX
* Sentence Transformers
* Tesseract OCR

whose tools made rapid prototyping possible.

---

## License

This project is released under the MIT License.

See the LICENSE file for details.

---

**Industrial Knowledge Copilot**
**ET AI Hackathon 2026 Submission**
**Team ParthPariwandh | Jadavpur University**
