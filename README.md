# Algorithm for Information Retrieval

## Overview
A comprehensive implementation of information retrieval algorithms including Boolean Search, PageRank, and Vector Space Models. This project demonstrates various IR techniques through practical applications.

## Projects

### 1. Boolean Search Engine (prob1)
An advanced search engine implementation using the 20 Newsgroups dataset.

**Features:**
- Boolean query processing (AND, OR, NOT)
- TF-IDF ranking system
- Dark mode interface
- Document snippets
- Full document view
- Zone-based indexing

**Usage:**
```bash
cd prob1
python app.py
# Access at http://localhost:5002
```

### 2. PageRank Simulator (prob2)
Interactive visualization of the PageRank algorithm.

**Features:**
- Real-time PageRank computation
- Interactive graph manipulation
- Convergence visualization
- Dynamic edge management
- Score history tracking

**Usage:**
```bash
cd prob2
python app.py
# Access at http://localhost:5001
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/Algorithm-for-information-retrieval.git
cd Algorithm-for-information-retrieval
```

2. Create and activate virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Linux/Mac
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Project Structure
```
.
├── prob1/
│   ├── app.py              # Boolean search implementation
│   ├── templates/          # HTML templates
│   │   ├── index.html     # Search interface
│   │   └── document.html  # Document view
│   └── static/            # CSS and assets
├── prob2/
│   ├── app.py             # PageRank simulator
│   ├── pagerank.py        # PageRank implementation
│   ├── templates/         # HTML templates
│   └── static/            # Visualization assets
└── requirements.txt       # Project dependencies
```

## Technical Implementation

### Boolean Search Engine
- **Indexing:** Inverted index with term frequencies
- **Query Processing:** Boolean operators (AND, OR, NOT)
- **Ranking:** TF-IDF scoring with document length normalization
- **Interface:** Flask-based web application

### PageRank Simulator
- **Algorithm:** Power iteration method
- **Parameters:**
  - Damping factor: 0.85
  - Convergence threshold: 1e-6
- **Visualization:** Real-time graph updates using NetworkX

## Dependencies
- Flask==2.0.1
- numpy==1.21.0
- scikit-learn==0.24.2
- networkx==2.6.2
- matplotlib==3.4.2
- nltk==3.6.2

## Development Setup
1. Install development dependencies:
```bash
pip install -r requirements-dev.txt
```

2. Run tests:
```bash
python -m pytest tests/
```

3. Start development server:
```bash
python app.py
```

## Contributing
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Authors
- Jeevan kumar U (github.com/JeevanKumar-u)

## Acknowledgments
- 20 Newsgroups dataset from scikit-learn
- NetworkX team for graph algorithms
- Flask framework developers
