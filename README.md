# Generative AI Experiments

Hands-on experiments with text, image and music generation using open-source models from Hugging Face. Each notebook runs end-to-end in Google Colab (GPU recommended for image and music).

## What's inside

| Project | Model / Stack | Open in Colab |
|---------|---------------|---------------|
| **Text generation** | GPT-2 via `transformers` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GOKUL-AI-tech/Generative-AI-Experiments/blob/main/notebooks/text-generation-gpt2.ipynb) |
| **Image generation** | Stable Diffusion v1.5 via `diffusers` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GOKUL-AI-tech/Generative-AI-Experiments/blob/main/notebooks/image-generation-stable-diffusion.ipynb) |
| **Music generation** | MusicGen-small (`facebook/musicgen-small`), WAV export | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GOKUL-AI-tech/Generative-AI-Experiments/blob/main/notebooks/music-generation-musicgen.ipynb) |
| **Gradio UI for GPT-2 (v1)** | GPT-2 + Gradio web interface | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GOKUL-AI-tech/Generative-AI-Experiments/blob/main/notebooks/gradio-ui-gpt2-v1.ipynb) |
| **Gradio UI for GPT-2 (v2)** | Refined Gradio chat-style UI | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GOKUL-AI-tech/Generative-AI-Experiments/blob/main/notebooks/gradio-ui-gpt2-v2.ipynb) |
| **Rule-based chatbot** | Flask + NLTK REST API | see below |

## Repository layout

```
notebooks/   # Colab notebooks (text, image, music, Gradio UIs)
chatbot/     # Flask + NLTK chatbot API
```

## Run the chatbot API locally

```bash
cd chatbot
pip install -r requirements.txt
python chatbot.py
```

Then send a message:

```bash
curl -X POST http://127.0.0.1:5000/chat \
     -H "Content-Type: application/json" \
     -d '{"message": "hello"}'
```

## Tech stack

Python · PyTorch · Hugging Face Transformers & Diffusers · Gradio · Flask · NLTK · Google Colab

## Author

**Gokul G** – B.Sc. AI & ML · [GitHub](https://github.com/GOKUL-AI-tech) · [LinkedIn](https://www.linkedin.com/in/gokul-g-ai-ml)
