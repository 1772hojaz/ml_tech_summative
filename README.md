# 📚 Agric Chatbot: T5 Model Fine-Tuning and Evaluation

This project explores the fine-tuning of a T5-small model for building an agricultural question-answering chatbot using a real-world farmers' query dataset. The chatbot is designed to assist farmers by providing contextual responses to common agricultural problems.

---

## 🧪 Experiments Summary

We fine-tuned multiple versions of the T5 model by adjusting various hyperparameters such as learning rate, batch size, weight decay, number of epochs, and precision mode. Evaluation was conducted using standard NLP metrics like **BLEU**, **ROUGE-1**, **ROUGE-2**, **ROUGE-L**, and **Evaluation Loss**.

### 🔍 First Model (Baseline)

| Metric        | Value    |
|---------------|----------|
| Eval Loss     | 2.6624   |
| BLEU          | 0.0680   |
| ROUGE-1       | 0.3217   |
| ROUGE-2       | 0.1737   |
| ROUGE-L       | 0.3173   |

---

## ✅ Best Performing Model: Mixed Precision

After experimenting with different settings, the **Mixed Precision model** showed the highest performance:

| Metric        | Value    | Improvement over Baseline |
|---------------|----------|----------------------------|
| Eval Loss     | 1.4469   | 🔻 46%                     |
| BLEU          | 0.2010   | 🔺 196%                    |
| ROUGE-1       | 0.4822   | 🔺 50%                     |
| ROUGE-2       | 0.3462   | 🔺 99%                     |
| ROUGE-L       | 0.4762   | 🔺 50%                     |

---

## 📈 Analysis

- The **Mixed Precision** model performed significantly better across all key evaluation metrics.
- It reduced evaluation loss by nearly half, which suggests better generalization.
- BLEU and ROUGE scores — which assess text similarity to human answers — improved dramatically, confirming better quality responses.
- Mixed precision also improved training efficiency by utilizing less memory and faster computation.

---

## 📦 Conclusion

This experiment proves that strategic hyperparameter tuning and enabling mixed precision training can **greatly improve model performance** in real-world text generation tasks such as chatbot systems. The final model is ready for deployment or integration into agricultural advisory platforms.

---

## 📁 Project Structure

- `mltech1.ipynb`: Main notebook with preprocessing, training, evaluation
- `data/`: Cleaned and preprocessed dataset
- `models/`: Saved versions of fine-tuned models
- `README.md`: This file

---

## ✨ Future Work

- Integrate the chatbot into a mobile/web application.
- Support multi-lingual and dialect-based inputs.
- Enable real-time retraining from user feedback.

---
## Link to Front-End Repo
https://github.com/1772hojaz/Machine_learning_techniques

---

📌 _Developed by Humphrey Nyahoja — Fine-tuning transformers to empower agriculture in Africa._

