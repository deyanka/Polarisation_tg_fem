# Feminism Polarization Analysis in Telegram

![Telegram Logo](https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg)

## 📌 Project Overview
This research analyzes affective and structural polarization between feminist and anti-feminist communities on Telegram during 2024-2025. Using NLP and social network analysis, I examine:
- Sentiment patterns in 78,029 posts/comments
- Network structures of 11,311 users across 8 channels
- Polarization metrics between the groups

**Key Findings**:
- Anti-feminist channels show 6x more negative sentiment (-0.61 vs -0.1)
- Only 0.04% users engage in heterophilic interactions
- Strong structural polarization with isolated "echo chambers"

## 🛠️ Methodology

### 1. Data Collection
In this part the data is parsed from Telegram API and the following information was gathered:
- Post texts and metadata (timestamps, authors)
- Comment texts with user identifiers
- Channel cross-references (mentions/forwards)

### 2. Sentiment Analysis
In this part a pretrained BERT-based model (RuBERT) is implemented to:
- Calculate sentiment of each individual comment
- Compute polarization and sentiment scores for each channel

### 3. User's Graph
In this part the user's graph is constructed to evaluate:
- Degree of homophily in interactions
- Cross-community engagement 

### 4. Channel's Graph
In this part channel's graph is constructed to analyze:
- Information flows between communities
- Articulation points in the network
- Foci overlap metrics

### 5. Network Analysis
In this part we calculate key graph properties:
- Degree distribution 
- Betweenness centrality (critical nodes identification)
- Foci overlap (cross-community interaction analysis)