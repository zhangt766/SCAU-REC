# SCAU-Rec: Subspace-Constrained Adapter Updates for LLM-Based Recommendations

This repository contains the implementation of **SCAU-Rec**, a continual low-rank adaptation framework for streaming recommendation with Large Language Models (LLMs).

---

## Files

```text
SCAU-Rec/
├── data/
│   ├── data_interface.py     # Data interface and dataloader utilities
│   ├── movielens_data.py     # MovieLens sequential dataset processing
│
├── model/
│   ├── model_interface.py    # Core model wrapper for adapter updating
│   ├── clara_utils.py        # Subspace projection and continual update utilities
│
└── README.md
```

---

## Preparation

1. Prepare the environment:

   ```sh
   git clone <anonymous-repo-url>
   cd SCAU-Rec
   pip install -r requirements.txt
   ```

2. Prepare the pre-trained Hugging Face model of LLaMA2-7B:

   - Download the LLaMA2-7B model from Hugging Face: `meta-llama/Llama-2-7b-hf`.

---

## Train SCAU-Rec

Train the adapter from scratch under the streaming protocol:

```bash
python model/model_interface.py
```
