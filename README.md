# 🧠 Sound-to-Shape Mapping: A Deep Learning Model of the Bouba-Kiki Effect

This project models the **Bouba-Kiki effect**—a well-known phenomenon in cognitive science where people consistently associate certain sounds with specific shapes (e.g., “bouba” with roundness, “kiki” with sharpness). My final-year thesis at NTU Singapore bridges **phonetic embeddings** and **visual representation** using **deep learning and phoneme-aware linguistic features**.

---

## 🔍 Project Objective

To design a deep learning pipeline that predicts how “bouba” or “kiki”-like a word sounds based on its phonemic structure, and uses this to generate a corresponding **abstract shape**—realizing a **word-to-shape** model grounded in cross-modal perception.

---

## 💡 Highlights

- 📚 **Dataset Creation**
  - Integrated phoneme-level transcriptions using CMU Pronouncing Dictionary
  - Annotated over 600 pseudowords with Bouba-Kiki scores from peer-reviewed studies
  - Extracted phoneme-based features (e.g., plosives, nasals, front/back vowels)

- 🧠 **Model Architecture**
  - Custom **BiLSTM model** trained to predict a boubaness score from phoneme sequences
  - Trained using Keras with early stopping and dropout for generalization
  - Achieved strong correlation between predicted scores and human judgments

- 🖌️ **Shape Generator**
  - Translates predicted boubaness into geometric forms based on perceptual shape rules
  - Parameters include: edge count, roundness, symmetry, irregularity
  - Generates visuals using Matplotlib and NumPy

- 🧪 **Evaluation**
  - Human participant study (N = 17) with shape–pseudoword matching task
  - **73.5% accuracy** in alignment between generated shapes and user intuition

---

## 📁 Repository Contents

- `FYP Code.ipynb` — Full training + generation pipeline (phoneme → score → shape)  
- `Bouba_Kiki_with_Phonemes.csv` — Labeled dataset with pseudowords and phoneme features  
- `final_model.h5` / `final_model.keras` — Trained BiLSTM model weights  
- `FYP Published Report.pdf` — Complete thesis report with references, architecture, and user study results  

---

## 🛠️ Technologies Used

- Python, NumPy, Pandas  
- Keras (TensorFlow backend)  
- CMUdict (via `pronouncing` library)  
- Matplotlib (shape rendering)  
- Scikit-learn, NLTK

---

## 🎯 Key Takeaways

This project demonstrates my ability to:

- Build **interpretable deep learning models** from scratch  
- Translate interdisciplinary research into deployable ML tools  
- Work with **sequence modeling** (BiLSTM, phonemes) and **visual generation**  
- Conduct and analyze **human evaluation experiments**  
- Combine **linguistic theory, cognition, and AI** into a unified system

---

## 👨‍💻 Author

**Tathagato Mukherjee**  
BSc (Hons), Data Science & AI, NTU Singapore  

---
