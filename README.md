# AI Code Explainer

This project allows users to input code snippets written in Python, C, C++, or Java and get plain-English explanations powered by a large language model (LLM). It is ideal for beginners learning to program. The interface is built using Gradio and runs entirely in Google Colab with GPU support.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vars16/AI-Code-Explainer/blob/main/AI%20Code%20Explainer.ipynb)

---

## Features

- AI-powered code explanation using DeepSeek model
- Clean and user-friendly Gradio interface with pastel purple theme
- Language selection dropdown for better context (Python, C, C++, Java)
- Example code snippets to try instantly
- Live code editor with syntax highlighting
- Plain-English explanation covering:
  - Purpose of the code
  - Key components and logic
  - Expected output
  - Sample use cases
- Options to download or copy the code
- Runs directly in Google Colab (GPU required)
- Free and open-source

---

## Try It Live

Click the badge above or open directly:  
https://colab.research.google.com/github/vars16/AI-Code-Explainer/blob/main/AI%20Code%20Explainer.ipynb

---

## How to Use (Colab)

1. Click the "Open in Colab" badge above.
2. Go to **Runtime > Change runtime type**.
3. Set **Hardware accelerator** to **GPU** (T4 or better recommended).
4. Click **Runtime > Run all**.
5. Wait for the model to load. Once ready, a Gradio interface will appear.
6. Input your code, choose the language, and click **Explain Code**.

> Important: This notebook requires a GPU.  
> To avoid errors, go to **Runtime > Change runtime type** and select **GPU** before running.

---

## Screenshots

_You can include screenshots of the interface here._

Example:

- Screenshot 1: Code input interface with language dropdown
- Screenshot 2: Plain-English explanation output
- Screenshot 3: Gradio UI with download and copy buttons

---

## Running Locally

This project runs as a Jupyter notebook. To run it locally:

1. Clone the repository:
```bash
git clone https://github.com/yourusername/AI-Code-Explainer.git
cd AI-Code-Explainer
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Launch the notebook:
```bash
jupyter notebook
```

> This notebook **requires a GPU** with at least 10 GB VRAM.  
> It may fail or run very slowly on CPU.

---

## Important Notes for Local Use

This notebook uses the `deepseek-ai/deepseek-coder-6.7b-instruct` model, which:

- Requires a **GPU with at least 10 GB VRAM** (e.g., T4, V100, A100)
- Will **not work** on most CPUs due to `bitsandbytes` GPU quantization
- May run **extremely slowly** or crash if run on CPU

We strongly recommend using **Google Colab with GPU enabled**, or a local machine with a **CUDA-enabled GPU**. If your laptop or desktop has a compatible GPU, you may try running it locally using the instructions above.

---

## License

This project is open-source under the [MIT License](LICENSE).
