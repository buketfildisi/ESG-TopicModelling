# 🌍 ESG Topic Modelling with Structured and Unstructured Sustainability Data

This repository documents the methods and results of the study "Integrating AI-Driven Analytics for Enhanced ESG Mapping: Aligning Local and Global Perspectives". The paper is currently under submission.

## 🧠 Project Overview

This project presents an AI-driven framework for analyzing sustainability discourse across **structured** (IMF Global Stability Reports) and **unstructured** (Greenstone LinkedIn newsletters) sources.

We apply and compare topic modelling methods:

- **LDA (Latent Dirichlet Allocation)**
- **BERTopic**
- **GenAI** (OpenAI GPT-4o-mini via LangChain)  
  ↳ with **Prompt Optimization via DSPy (MIPROv2)**

**Evaluation Metrics**:  
✔️ Coherence  
✔️ Diversity  
✔️ Semantic Similarity  

Our goal is to uncover ESG-related insights, enhance SDG alignment, and deliver interpretable, sector- and region-specific sustainability intelligence.

## ⚙️ Setup and Installation

To replicate this study, please follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/buketfildisi/ESG-TopicModelling.git](https://github.com/buketfildisi/ESG-TopicModelling.git)
    cd your-repo-name
    ```
2.  **Create and activate a virtual environment (recommended):**
    ```bash
    python -m venv venv
    # On Windows:
    # .\venv\Scripts\activate
    # On macOS/Linux:
    # source venv/bin/activate
    ```
3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    * **Note:** This project was developed and tested with Python 3.11. Ensure you have a compatible Python version installed.

4.  **OpenAI API Key (for GenAI/GPT-4o-mini):**
    If you intend to run the GenAI models (GPT-4o-mini and gpt-3.5-turbo), you will need an OpenAI API key.
    * Set your API key as an environment variable (replace with your actual key):
        
OPENAI_API_KEY="your_openai_api_key_here"


## 📁 Repository Structure
├── CODES # Python notebooks and scripts for data scraping, topic modelling, cosine similarity, optimisation and evaluation
├── DATA #  IMF reports and Greenstone newsletters
├── RESULTS # Extracted topics, visualisations, and metric outputs


## 📊 Data Sources

- **Structured**: 41 IMF Global Financial Stability Reports (2003–2023)
- **Unstructured**: 62 Greenstone LinkedIn newsletters on sustainability (2022–2023)
  
 ### Data Availability and Acquisition:

Full datasets are provided in the `DATA/samples/` directory to facilitate understanding of the data format and to test the code's functionality.

* **IMF Global Financial Stability Reports:** These reports are publicly available on the International Monetary Fund's official website. Our data was programmatically extracted from the PDF versions of these reports. [https://www.imf.org/en/Publications/GFSR]
* **Greenstone LinkedIn Newsletters:** These newsletters were collected directly from Greenstone's public LinkedIn page. As they are publicly accessible posts, their use for research purposes falls within fair use guidelines. [https://www.linkedin.com/newsletters/esg-sustainability-insights-6914225915384279040/]

**Disclaimer on Copyright:**
While the IMF reports are publicly available, their use should adhere to IMF's terms of use. The LinkedIn newsletter data, being publicly accessible, is used for research purposes in line with academic fair use principles. We do not claim ownership of the data. For full replication requiring the complete datasets, users would need to acquire them from their respective original sources.

## 📈 Interactive Dashboard

Explore findings interactively via Looker Studio:  
🔗 [Open Dashboard](https://lookerstudio.google.com/s/l6pEtcAAgd0)

## 📄 Citation

If you use this work, please cite our paper (link will be added upon publication).

## 📬 Contact

For questions, feedback, or collaboration, contact:  
buketfildisi@gmail.com or buket.fildisi@mail.bcu.ac.uk
