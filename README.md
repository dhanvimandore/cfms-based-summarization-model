📄 CFMS: Consistency-Aware Multi-Document Summarization

A research-driven framework for multi-document summarization (MDS) that improves factual consistency by explicitly modeling agreement across multiple news sources.

🚀 Overview

In real-world scenarios, the same event is reported by multiple news sources with variations in wording, emphasis, and factual detail. This leads to:

Information redundancy
Conflicting narratives
Cognitive overload for users

This project proposes CFMS (Consistency-Focused Multi-Source Summarization), a novel framework that introduces structured cross-source reasoning to generate reliable and coherent summaries.

🧠 Key Contributions
📌 Introduced CFMS framework for consistency-aware summarization
📌 Explicit modeling of cross-source agreement
📌 Designed Cross-Source Alignment, Consistency Scoring, and Factual Attention
📌 Built NewsSumm++ dataset pipeline for Indian English news
📌 Achieved strong performance on ROUGE and BERTScore
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

A custom dataset designed for multi-document summarization in Indian English news.

🔹 Statistics
45,284 Articles
387 Event Clusters
Multi-source news aggregation
🔹 Pipeline
Data Collection
Cleaning
Deduplication (FAISS)
Semantic Filtering
Event Clustering
Quality Filtering
Dataset Structuring
⚙️ Tech Stack
Python
PyTorch
HuggingFace Transformers
FAISS
Google Colab / Local Environment
▶️ Usage
🔹 Train Model
python train.py
🔹 Generate Summary
python generate.py --input "path_to_documents"
📈 Results
Metric	Score
ROUGE-1	0.3903
ROUGE-2	0.1954
ROUGE-L	0.3305
BERTScore	0.8803
🔍 Model Insight

CFMS improves factual consistency by prioritizing information that appears across multiple sources, making summaries:

More reliable
Less redundant
Better aligned with real-world facts
⚠️ Limitations
Computationally intensive
Requires high-quality clustered data
Token-level alignment may truncate long inputs
Training stability depends on dataset size
🔮 Future Work
Hybrid model (CFMS + Hierarchical architecture)
Real-time summarization
Multilingual extension
Graph-based cross-document reasoning
🧪 Demo

Run the demo:

open cfms_demo.html
👩‍💻 Author

Dhanvi Mandore
MIT World Peace University, Pune

🤝 Acknowledgment

This work was developed with support from:

Suvidha Foundation
📜 Citation
@article{mandore_cfms_2026,
  title={CFMS: Consistency-Aware Multi-Document Summarization},
  author={Mandore, Dhanvi},
  year={2026},
  institution={MIT World Peace University},
  {Suvidha Foundation, Nagpur}
}
📜 License

For academic and research purposes only.
