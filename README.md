# GPT-3.5-Hallucination-Detector-Fast-AI-week-2-

I built this to catch GPT-3.5 when it makes things up. It’s a BERT-based classifier trained on ~30k examples of AI hallucinations (HaluEval).

Try the Live Demo on Hugging Face: https://huggingface.co/spaces/jaredcobrin/ai-lie-detector 

The Project

For Week 2 of fast.ai, I moved from a Kaggle notebook to a live deployment. I chose BERT because its bidirectional nature is perfect for catching the subtle context clues that signal an AI is "guessing" rather than retrieving facts.

What I Learned

Safetensors: I exported the model in .safetensors format. It's the modern standard because it's secure (no "pickle" code execution) and loads much faster.

Factual Consistency: Working with the HaluEval dataset taught me how to identify "linguistic smells"—the specific ways LLMs sound confident even when they are wrong.

Production MLOps: I learned how to bridge the gap between training in a lab (Kaggle) and building a usable interface (Gradio/Hugging Face).

Tech Stack

Engine: PyTorch / fast.ai

Model: BERT-base-uncased

Deployment: Hugging Face Spaces & Gradio

Format: Safetensors

The Goal

My main focus is AI alignment and reducing the risk of a disaster from misaligned models. Developing tools that can verify if an AI is telling the truth is a small but necessary step toward building safe, reliable systems.
