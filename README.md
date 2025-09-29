# Stock Co-Investment Network Analysis: Microsoft Focus (2016-2023)

## Overview

This project analyzes stock co-investment networks with a specific focus on Microsoft (MSFT) from 2016 to 2023, conducted as part of the **Data-driven Business & Behaviour Analytics** coursework at the **University of Edinburgh**. The analysis examines how Microsoft connects with investors and other stocks through network analysis techniques, revealing patterns of diversification, sector clustering, and the impact of the COVID-19 pandemic on investment behaviors.

## 📊 Key Findings

- **MSFT's Dual Role**: Microsoft functions both as a technology sector hub and as a bridge connecting different market sectors
- **Pandemic Impact**: Significant shifts in investor confidence and network structure during COVID-19 (2020-2021)
- **Community Evolution**: Dynamic changes in Microsoft's investment communities across different market periods
- **Centrality Analysis**: Microsoft consistently maintains high centrality measures, indicating its importance in the investment network

## 🎯 Research Objectives

1. **Network Construction**: Build bipartite networks representing investor-stock relationships
2. **Projection Analysis**: Create stock-side projections to understand co-investment patterns
3. **Ego Network Study**: Analyze Microsoft's direct investment neighborhood
4. **Temporal Analysis**: Track network evolution before, during, and after the COVID-19 pandemic
5. **Community Detection**: Identify investment communities and Microsoft's role within them
6. **Correlation Analysis**: Use spanning trees to analyze stock correlation structures

## 📁 Project Structure

```
stock-analysis/
├── dataset/
│   ├── Stock_Prices/
│   │   └── stock_prices.csv          # Historical stock price data
│   └── Temporal_Data/
│       ├── 2016_Q1.xlsx - 2023_Q2.xlsx  # Quarterly investor-stock data
├── stock analysis.ipynb              # Main analysis notebook
├── S2714494.pdf                      # Project report
└── README.md                         # This file
```

## 🛠️ Methodology

### 1. Network Construction
- **Bipartite Networks**: Investors and stocks as two distinct node sets
- **Edge Weights**: Frequency of investor-stock relationships
- **Temporal Segmentation**: Quarterly analysis from 2016 Q1 to 2023 Q2

### 2. Network Projections
- **Stock-Side Projection**: Co-investment relationships between stocks
- **Weighted Edges**: Number of shared investors between stock pairs
- **Network Filtering**: Threshold-based edge filtering for clarity

### 3. Ego Network Analysis
- **Microsoft-Centered**: Focus on MSFT's direct connections
- **Comparative Analysis**: Bipartite vs. unipartite ego networks
- **Density Metrics**: Network density and clustering coefficients

### 4. Community Detection
- **Louvain Algorithm**: Optimal community partitioning
- **Girvan-Newman Algorithm**: Hierarchical community structure
- **Modularity Analysis**: Community strength measurement

### 5. Centrality Measures
- **Degree Centrality**: Node connectivity importance
- **Betweenness Centrality**: Bridge node identification
- **Closeness Centrality**: Network accessibility measures
- **Eigenvector Centrality**: Influence-based importance

### 6. Spanning Tree Analysis
- **Minimum Spanning Tree**: Correlation-based stock relationships
- **Distance Metric**: √(2(1-correlation)) for stock pairs
- **Temporal Comparison**: Pre-pandemic, during, and post-pandemic periods

## 📈 Key Results

### Network Statistics Evolution
- **Nodes**: ~1,500 stocks across different quarters
- **Edges**: ~100,000+ co-investment relationships
- **Density**: ~0.093 (relatively sparse network)
- **Clustering**: High local clustering indicating sector groupings

### Microsoft's Network Position
- **Ego Network Size**: 870 directly connected stocks
- **Degree**: 869 connections in the full network
- **Community Membership**: Consistently appears in large, diverse communities
- **Centrality Rankings**: High scores across all centrality measures

### Pandemic Impact (2020-2021)
- **Network Fragmentation**: Increased modularity during pandemic
- **Community Size Changes**: Microsoft's community composition shifts
- **Correlation Patterns**: Different spanning tree structures across periods
- **Hub Transitions**: Changes in most central nodes during crisis

### Community Analysis
- **Sector Clustering**: Technology stocks form tight communities
- **Cross-Sector Bridges**: Microsoft connects tech with traditional sectors
- **Temporal Stability**: Some communities persist while others evolve
- **Top Co-occurring Stocks**: AAPL, GOOGL, AMZN frequently in MSFT communities

## 🔧 Technologies Used

- **Python 3.x**
- **NetworkX**: Network analysis and graph algorithms
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Matplotlib & Seaborn**: Data visualization
- **Scikit-learn**: Additional analysis tools

## 📊 Visualizations

The project includes comprehensive visualizations:
- Bipartite network layouts
- Ego network structures
- Temporal evolution plots
- Community heatmaps
- Spanning tree diagrams
- Centrality measure comparisons

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy networkx matplotlib seaborn openpyxl
```

### Running the Analysis
1. Clone this repository
2. Ensure all data files are in the correct directories
3. Open `stock analysis.ipynb` in Jupyter Notebook
4. Run cells sequentially for complete analysis

### Data Requirements
- Quarterly investor-stock relationship data (Excel format)
- Historical stock price data (CSV format)
- Data spans from 2016 Q1 to 2023 Q2

## 📚 Academic Context

**Course**: Data-driven Business & Behaviour Analytics  
**Institution**: University of Edinburgh  
**Academic Year**: 2023-2024  
**Focus**: Network analysis applied to financial markets

## 🔍 Future Research Directions

- **Extended Time Series**: Analysis beyond 2023
- **Sector-Specific Studies**: Deep dive into technology sector dynamics
- **Risk Analysis**: Correlation between network position and stock volatility
- **Prediction Models**: Using network features for investment recommendations
- **International Markets**: Comparative analysis across global markets

## 📝 References

The analysis builds upon established network theory and financial market research, applying graph theory concepts to understand co-investment patterns and market structure evolution.

## 📄 License

This project is part of academic coursework and is intended for educational purposes.

---

