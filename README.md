# APGNN-SNA-Hybrid-Recommendation-System

## Abstract

This project presents a groundbreaking hybrid computational framework that systematically integrates **Personalized Graph Neural Networks with Attention Mechanism (A-PGNN)** and comprehensive **classical Social Network Analysis (SNA)** techniques for enhanced recommendation systems. Our approach addresses the fundamental limitations of modern graph neural networks in demonstrating traditional social network concepts while preserving their superior computational capabilities.

## 🎯 Key Results

- **18.2% improvement** in Hit Rate@5 (0.0187 → 0.0221)
- **16.9% improvement** in Mean Reciprocal Rank (0.0089 → 0.0104)
- **84.5% session retention rate** from temporal windowing
- **Complete SNA coverage** with all major centrality measures
- **4% plagiarism similarity** - ensuring original research contribution

## 🏗️ Project Pipeline

![Project Pipeline](assets/project_Pipeline.png)

Our hybrid approach follows a systematic 4-phase implementation:

1. **Phase 1: Foundation Setup** - Environment setup, dataset acquisition, and A-PGNN code analysis
2. **Phase 2: Core Implementation** - Session data preprocessing, basic SNA implementation, and initial A-PGNN testing
3. **Phase 3: Integration Development** - SNA feature engineering, model training, and hybrid architecture development
4. **Phase 4: Evaluation and Analysis** - Performance comparison, visualization generation, and comprehensive analysis


## 📊 Dataset

**MovieLens 100K Dataset**
- **100,000 ratings** from 943 users on 1,682 movies
- **Rating scale**: 1-5 stars
- **Temporal span**: September 1997 to April 1998
- **Network density**: 0.0290 (typical sparse recommendation data)
- **Sessions created**: 2,280 with 84.5% retention rate

## 🔬 Technical Approach

### Classical SNA Features
- **Degree Centrality**: Local connectivity measurement
- **Betweenness Centrality**: Bridge identification in network
- **Closeness Centrality**: Global accessibility assessment
- **PageRank**: Importance through random walk models

### A-PGNN Enhancement
- Session-based temporal analysis using 24-hour windows
- Gated graph convolution with attention mechanisms
- Feature integration through linear transformation and concatenation
- Multi-head attention for personalized recommendations

### Hybrid Integration
- Dual-pathway processing: sessions + bipartite graphs
- SNA feature vectors (6-dimensional) combined with neural embeddings
- Enhanced architecture maintaining both performance and interpretability

## 📈 Performance Comparison

| Model | Hit Rate@3 | Hit Rate@5 | MRR | NDCG@5 |
|-------|------------|------------|-----|--------|
| Baseline A-PGNN | 0.0145 | 0.0187 | 0.0089 | 0.0156 |
| **Enhanced A-PGNN+SNA** | **0.0189** | **0.0221** | **0.0104** | **0.0184** |
| **Improvement** | **+30.3%** | **+18.2%** | **+16.9%** | **+17.9%** |

## 🛠️ Technologies Used

- **Platform**: Google Colab with T4 GPU
- **Deep Learning**: PyTorch 2.6.0+cu124
- **Graph Processing**: DGL 2.4.0
- **Network Analysis**: NetworkX 3.5+
- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn



