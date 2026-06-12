# Fine-Tuning TinyLLaMA for Text Simplification (WikiLarge)

This project fine-tunes the TinyLLaMA language model on the WikiLarge dataset to perform **text simplification**, converting complex academic sentences into simpler, more readable English.

---

## 🚀 Project Overview

- Base Model: TinyLLaMA (~1.1B parameters)
- Fine-tuning Method: LoRA (Parameter-Efficient Fine-Tuning)
- Dataset: WikiLarge (123,862 training samples)
- Task: Text Simplification

---

## 🧠 Objective

To transform complex, academic-level sentences into simple, human-readable text while preserving meaning.

---

## 🧪 Training Setup

- Framework: PyTorch + Hugging Face Transformers
- GPU: NVIDIA RTX 3060 Laptop GPU (6GB VRAM)
- Trainable Parameters: ~1.13%
- Precision: Mixed precision training enabled

---

## 📊 Results

- Training Loss: ~1.03
- Evaluation BLEU: ~0.0159
- Readability Improvement (FRE): +76.5 points

The model significantly improves readability, though further optimization is required for semantic accuracy.

---

## 📌 Example Output

**Input (Complex):**
The prominent clinician conceptualized a novel therapeutic strategy to mitigate the deleterious effects of the pathogen.

**Output (Simplified):**
This is an example of the common practice in medicine whereby a physician may use a less complex approach.

---

## ⚠️ Limitations

- Low BLEU score indicates limited semantic preservation
- Occasional hallucination in generated text
- Needs further training with instruction-based formatting

---

## 🔧 Future Improvements

- Add SARI + ROUGE evaluation metrics
- Improve instruction-based fine-tuning format
- Increase LoRA rank for better performance
- Reduce hallucination using better alignment methods

---

## 📂 Dataset

- WikiLarge dataset for text simplification

---

## 👨‍💻 Author

Mohsin Raza  
GitHub: https://github.com/Mohsindahri

---

## 📜 License

For academic and research use only.
