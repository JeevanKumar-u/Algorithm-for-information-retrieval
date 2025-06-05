# Algorithm for Information Retrieval (AFIR)

## Overview
A comprehensive suite of information retrieval systems implementing various search, ranking, and retrieval algorithms across different use cases.

## Projects

### 1. Boolean Search Engine with TF-IDF (prob1)
Advanced document retrieval system using the 20 Newsgroups dataset.

**Features:**
- Boolean query operators (AND, OR, NOT)
- TF-IDF scoring with document length normalization
- Dark mode user interface
- Document snippets and full-text view
- Zone-based indexing (title, body)

**Usage:**
```bash
cd prob1
python app.py
# Access at http://localhost:5002
```

### 2. PageRank Simulator (prob2)
Interactive visualization tool for PageRank algorithm.

**Features:**
- Real-time PageRank computation
- Dynamic graph manipulation
- Convergence visualization
- Edge addition/removal
- Score history tracking

**Usage:**
```bash
cd prob2
python app.py
# Access at http://localhost:5001
```

### 3. Multimodal Search Engine (prob3)
Combined image and text search system for the Flickr8k dataset.

**Features:**
- Visual similarity using ResNet18
- Text similarity with BERT embeddings
- Color histogram analysis
- Interactive result refinement
- Cross-modal retrieval

**Usage:**
```bash
cd prob3
python multimodal_app.py
# Access at http://localhost:5003
```

### 4. Question Answering System (prob4)
Neural QA system with knowledge base integration.

**Features:**
- BERT-based answer extraction
- Named Entity Recognition
- Document retrieval using BM25
- Answer confidence scoring
- Source attribution

**Usage:**
```bash
cd prob4
python qa_system.py
# Access at http://localhost:5004
```

### 5. Neural-Traditional Hybrid Search (prob5)
Comparative search system combining classical and neural approaches.

**Features:**
- Traditional search (BM25, TF-IDF)
- Neural search with transformers
- Visual result comparison
- Performance analysis tools
- ColBERT implementation

**Usage:**
```bash
cd prob5
python hybrid_search.py
# Access at http://localhost:5005
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/AFIR.git
cd AFIR
```

2. Create virtual environment:
```bash
python -m venv venv
source venv/bin/activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Project Structure
```
AFIR/
├── prob1/                  # Boolean Search Engine
│   ├── app.py
│   ├── templates/
│   └── static/
├── prob2/                  # PageRank Simulator
│   ├── app.py
│   ├── pagerank.py
│   └── templates/
├── prob3/                  # Multimodal Search
│   ├── multimodal_app.py
│   ├── models/
│   └── data/
├── prob4/                  # Question Answering
│   ├── qa_system.py
│   ├── knowledge_base/
│   └── models/
├── prob5/                  # Hybrid Search
│   ├── hybrid_search.py
│   ├── evaluator/
│   └── models/
└── requirements.txt
```

## Dependencies
- Flask==2.0.1
- torch==1.9.0
- transformers==4.11.0
- networkx==2.6.2
- scikit-learn==0.24.2
- numpy==1.21.0
- matplotlib==3.4.2
- nltk==3.6.2
- spacy==3.1.0

## Development

1. Set up development environment:
```bash
pip install -r requirements-dev.txt
```

2. Run tests:
```bash
python -m pytest tests/
```

3. Start specific project:
```bash
cd probN  # N=1,2,3,4,5
python app.py
```

## Contributing
1. Fork the repository
2. Create feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open Pull Request

## License
MIT License - see [LICENSE](LICENSE)

## Authors
- Your Name (@githubusername)

## Acknowledgments
- 20 Newsgroups dataset (scikit-learn)
- Flickr8k dataset
- HuggingFace Transformers
- NetworkX team
