# 📊 SmartPPT: AI-Powered Presentation Architect

**SmartPPT** is an automated tool that transforms web content into professional PowerPoint presentations. By leveraging **Google Gemini 2.5 Flash** and **LangChain**, it scrapes data from URLs or Google Search results, summarizes key points, fetches relevant images, and injects them into a pre-designed `.pptx` template.

## 🧐 Problem Statement
Creating presentations is traditionally a time-consuming manual process. Researching topics, summarizing long articles, and sourcing high-quality, relevant images often takes hours. **SmartPPT** automates this workflow, allowing users to generate a structured, visually-aided draft in seconds from just a search query or a list of links.

## 🚀 Features & USP
* **🌐 Dual Input Modes:** Choose between providing specific URLs manually or letting the AI find relevant sources via Google Search integration.
* **🕷️ Intelligent Web Scraper:** Extracts text and image assets from complex HTML structures using **BeautifulSoup4**, with smart filtering for relevant visuals.
* **🧠 Gemini-Powered Summarization:** Uses Gemini 2.5 Flash to distill raw web data into concise, presentation-ready bullet points.
* **🖼️ Visual Integration:** Automatically maps discovered web images to specific slides based on content relevance.
* **🎨 Template Support:** Injects content into a master `.pptx` layout (**Bracket design.pptx**) to ensure professional branding and consistent formatting.

## 🧠 Technology Stack

| Component | Technology Used |
| :--- | :--- |
| **Frontend/UI** | Streamlit |
| **Orchestration** | LangChain (`langchain-google-genai`) |
| **AI Model** | Gemini 2.5 Flash (Google AI Studio) |
| **Search Engine** | Google Search API (`googlesearch-python`) |
| **PPT Logic** | `python-pptx` |
| **Web Scraping** | BeautifulSoup4 & Requests |

## 📂 Repository
```text
SmartPPT/
├── .streamlit/
│   └── secrets.toml     # Google API Key storage
|── .gitignore           # Git exclusion rules
|── Ai_ppt.py            # Main Application Script
├── Bracket design.pptx  # The base PowerPoint template used by the app
├── PPT.pptx             # Sample ppt on Independence Day
├── README.md            # Project Documentation
└── requirements.txt     # Python Dependencies
