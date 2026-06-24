# ChitroJera Multimodal VQA Framework 🇧🇩🤖

An end-to-end deep learning framework for geoculturally relevant Visual Question Answering (VQA) in Bangla. This project implements a Dual-Encoder architecture fusing text embeddings from **BanglaBERT** and visual embeddings from a **Vision Transformer (ViT)** using PyTorch.

## 🚀 Project Architecture
- **Language Encoder:** `csebuetnlp/banglabert` (Handles Bengali natural language questions)
- **Vision Encoder:** `google/vit-base-patch16-224-in21k` (Processes localized Bengali images)
- **Fusion Layer:** Late-fusion feature concatenation with a deep neural network classification head.

## 🧠 Pre-trained Model Weights
Due to GitHub's strict 100MB upload file limits, the trained **753 MB** model weights file (`chitrojera_dual_encoder.pt`) is safely hosted on the Hugging Face Model Hub.

👉 **[Download the Trained Weights on Hugging Face](https://huggingface.co/MSAkash/ChitroJera-Dual-Encoder-VQA)**

## 💻 How to Use This Project

1. **Clone the Repo:**
   ```bash
   git clone [https://github.com/YOUR_GITHUB_USERNAME/ChitroJera-Multimodal-VQA.git](https://github.com/skyline180/ChitroJera-Multimodal-VQA.git)
   ```
2. Open the Notebook:
Open `ChitroJera_VQA_Pipeline.ipynb` directly in Google Colab or locally with a GPU.
3. Run Inference:
Download the `chitrojera_dual_encoder.pt` file from the Hugging Face link above, drop it into your workspace directory, and use the provided `ask_chitrojera()` function to query your own images in Bangla!
