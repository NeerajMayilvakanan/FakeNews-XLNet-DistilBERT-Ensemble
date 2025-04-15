# FakeNews-XLNet-DistilBERT-Ensemble
This research uses XLNet and DistilBERT for fake news detection, applying ensemble methods (Simple Average and Majority Vote) on Politifact and GossipCop datasets. XLNet excels in Politifact, while ensembles boost accuracy, especially in celebrity news detection.

## 📊 Dataset

The study uses two datasets from the FakeNewsNet repository:

- **Politifact**: Fact-checked political articles.
- **GossipCop**: Celebrity news and gossip articles.

### Data Split:
- **80% Training**  
- **10% Validation**  
- **10% Testing**

This split ensures models generalize well on unseen data and are rigorously evaluated.

## 🧠 Models Used

- [XLNet](https://arxiv.org/abs/1906.08237)
- [DistilBERT](https://arxiv.org/abs/1910.01108)
- **Simple Average Ensemble**: Averaged predictions of XLNet & DistilBERT.
- **Majority Vote Ensemble**: Class prediction by majority agreement.

## 📏 Evaluation Metrics

The models were evaluated using:
- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**

These metrics were calculated separately on validation and testing datasets.

---

### 📈 Results Summary

#### Politifact Dataset

| Model | Accuracy | Precision | Recall | F1 Score |
|-------|----------|-----------|--------|----------|
| XLNet | 89.62% | 90.48% | 91.94% | 91.20% |
| DistilBERT | 87.74% | 94.55% | 83.87% | 88.89% |
| Simple Avg Ensemble | 88.68% | 94.64% | 85.48% | 89.83% |
| Majority Vote Ensemble | 88.68% | 96.30% | 83.87% | 89.66% |

#### GossipCop Dataset

| Model | Accuracy | Precision | Recall | F1 Score |
|-------|----------|-----------|--------|----------|
| XLNet | 85.50% | 89.67% | 91.33% | 90.49% |
| DistilBERT | 85.86% | 88.20% | 93.84% | 90.94% |
| Simple Avg Ensemble | **86.54%** | 88.78% | 94.08% | 91.35% |
| Majority Vote Ensemble | 84.87% | **90.94%** | 88.82% | 89.87% |

---

## 📊 Graph Insights

![image](https://github.com/user-attachments/assets/c2410b39-aa97-4ee2-b285-c08c5eedf6d6)
- **Graph 1**: XLNet achieves highest test accuracy on **Politifact** (89.62%)
![image](https://github.com/user-attachments/assets/1b388216-8700-42f8-ae94-e9ddc5299f45)
- **Graph 2**: Simple Avg Ensemble performs best on **GossipCop** (86.54%)
![image](https://github.com/user-attachments/assets/990b8250-3177-4731-809e-c9a8818db5fb)
- **Graphs 3–8**: Across all metrics, **Majority Vote Ensemble** showed consistent improvement, indicating ensembling helps reduce errors and improve generalization.

## ✅ Conclusion

This research highlights that:
- **XLNet** performs strongly on political fake news.
- **Simple Average Ensembles** work best on celebrity gossip datasets.
- **Majority Vote Ensemble** consistently balances precision and recall.
- A **multi-model approach** significantly enhances fake news detection reliability.

## License

This project is licensed under the terms of the **GNU General Public License v3.0** (GPL-3.0).

See the [LICENSE](LICENSE) file for details.

Copyright (C) 2025 NeerajMayilvakanan.
