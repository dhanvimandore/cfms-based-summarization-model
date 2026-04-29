📄 CFMS: Consistency-Aware Multi-Document Summarization

A research-driven framework for multi-document summarization (MDS) that enhances factual consistency by explicitly modeling agreement across multiple sources.

🚀 Overview

With the rapid growth of digital news platforms, the same event is often reported by multiple sources, leading to redundancy, inconsistency, and information overload.

CFMS (Consistency-Focused Multi-Source Summarization) addresses these challenges by introducing structured cross-source reasoning to generate reliable, coherent, and factually grounded summaries.

🧠 Key Features
Consistency-aware summarization
Cross-source agreement modeling
Reduced redundancy and hallucination
Improved factual reliability
Custom dataset pipeline (NewsSumm++)
🏗️ Architecture
Input Documents
      ↓
BART Encoder
      ↓
Cross-Source Alignment
      ↓
Consistency Scoring
      ↓
Factual Attention
      ↓
Flan-T5 Decoder
      ↓
Final Summary
📊 Dataset: NewsSumm++

A curated dataset for Indian English multi-document news summarization.

Highlights:
📄 45,284 articles
📚 387 event clusters
🌍 Multi-source news data
Pipeline:
Data Collection
Data Cleaning
Deduplication (FAISS-based)
Semantic Filtering
Event Clustering
Quality Filtering
Dataset Structuring
⚙️ Installation
git clone https://github.com/dhanvimandore/CFMS-Summarization.git
cd CFMS-Summarization
pip install -r requirements.txt
▶️ Usage
Train Model
python train.py
Generate Summary
python generate.py --input "path_to_documents"
📈 Results
Metric	Score
ROUGE-1	0.3903
ROUGE-2	0.1954
ROUGE-L	0.3305
BERTScore	0.8803
🔍 Model Comparison
Feature	CFMS	Hierarchical Models
Factual Consistency	High	Moderate
Scalability	Limited	High
Complexity	High	Low
Performance	Strong	Strong
⚠️ Limitations
High computational cost
Requires quality clustered data
Sensitive to noise in inputs
Token alignment constraints
🔮 Future Work
Multilingual summarization
Real-time processing
Hybrid architectures (CFMS + Hierarchical)
Graph-based cross-document reasoning
🧪 Demo

Run the demo:

open cfms_demo.html
🛠️ Tech Stack
Python
PyTorch
HuggingFace Transformers
FAISS
Google Colab / Local Environment
👩‍💻 Author

Dhanvi Mandore
MIT World Peace University, Pune

🤝 Acknowledgment

This work was carried out as part of an internship and research initiative supported by:

Suvidha Foundation

The author sincerely acknowledges the guidance, support, and resources provided by the organization during the development of this project.

📜 Citation

If you use this work, please cite:

@article{mandore_cfms_2026,
  title={CFMS: Consistency-Aware Multi-Document Summarization for Indian English News},
  author={Mandore, Dhanvi},
  year={2026},
  institution={Developed with support from Suvidha Foundation, Nagpur}
}
📜 License

This project is intended for academic and research purposes only.
