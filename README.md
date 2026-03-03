***

```markdown
# IIT Patna Research Internship: Video Harassment Detection

This repository documents my research internship project at **IIT Patna**, focused on building a dataset and developing LLM-based models to **identify and explain harassment incidents from videos**.

## 🎯 Project Overview

Developed a comprehensive pipeline for:
- Curating a harassment video dataset
- Implementing vision-language models (VLMs) for video analysis
- Performing basic data analysis and validation

**Core Objective**: Enable automated detection and explanation of harassment behaviors from real-world video footage.

## 📊 Dataset

 (https://huggingface.co/datasets/iamalekhya/Finance_set/blob/main/Finance_set.csv) 

## 🛠️ Implemented Models

| Model            | Notebook                                           | Parameters | Purpose                           |
|------------------|----------------------------------------------------|------------|-----------------------------------|
| **Qwen2-VL**     | [Qwen2_VL_7B.ipynb](Qwen2_VL_7B.ipynb)             | 7B         | Video understanding & description |
| **InternVL2**    | [InternVL2_5_8B.ipynb](InternVL2_5_8B.ipynb)       | 5.8B       | Multimodal video analysis         |
| **DeepSeek-VL2** | [DeepSeek_VL2.ipynb](DeepSeek_VL2.ipynb)           | -          | Video feature extraction          |
| **InternVideo2** | [InternVideo2_5_4B.ipynb](InternVideo2_5_4B.ipynb) | 5.4B       | Video classification              |
| **Aria**         | [Aria.ipynb](Aria.ipynb)                           | -          | Model comparison                  |

## 📁 Recent Work

- **Peak File Handling**: [Peak_file_handling.ipynb](Peak_file_handling.ipynb) - Data processing & peak detection
- **Short Videos (<30min)**: [&lt;30min_Videos.ipynb](%3C30min_Videos.ipynb) - Processing pipeline for short clips

## 🚀 Quick Start

All notebooks created using **Google Colab** for easy reproduction:

```bash
# Clone the repository
git clone https://github.com/AlekhyaGangopadhyay/IITPatna_Internship_LLMs.git

# Open any notebook in Colab or Jupyter
jupyter notebook Qwen2_VL_7B.ipynb
```
## 🛠️ Environment Setup

### Prerequisites
```bash
# Python 3.10+
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
pip install transformers accelerate
pip install huggingface_hub
pip install qwen-vl-utils
pip install flash-attn --no-build-isolation
pip install pillow
pip install opencv-python
pip install pandas numpy matplotlib seaborn

GPU Requirements
Minimum: NVIDIA GPU with 16GB VRAM (A100/T4 recommended)

Colab: T4 GPU sufficient for inference

Local: RTX 3090/4090 or A100

| Model        | Key Parameters     | Notes                            |
| ------------ | ------------------ | -------------------------------- |
| Qwen2-VL     | max_new_tokens=512 | Best for detailed descriptions   |
| InternVL2    | image_size=448     | Adjust based on video resolution |
| DeepSeek-VL2 | num_frames=32      | Extract 1fps from videos         |
## 📈 Key Contributions

1. **Dataset Creation**: Built structured CSV dataset from harassment videos
2. **Model Implementation**: Deployed 5+ state-of-the-art VLMs
3. **Data Analysis**: Video duration analysis, quality assessment
4. **Pipeline Development**: End-to-end video processing workflow

## 🔬 Research Context

**IIT Patna Research Internship** (2026)
- Mentors: [To be added]
- Focus: AI for social good - Harassment detection
- Tools: PyTorch, Hugging Face, Google Colab

## 📝 Future Work

- Model fine-tuning on harassment dataset
- Ensemble methods for improved accuracy
- Real-time inference pipeline
- Comprehensive evaluation metrics

## 🙏 Acknowledgments

- **IIT Patna** for the research opportunity
- Mentors for guidance on dataset creation
- Hugging Face for model hosting

---

**Contact**: Alekhya Gangopadhyay | [GitHub](https://github.com/AlekhyaGangopadhyay) [Email](iamalekhya7@gmail.com)
```

***

