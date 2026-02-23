# LLM Hands-On

This repository contains Jupyter notebooks for hands-on experiments with Large Language Models (LLMs). These notebooks are designed to be run easily in **Google Colab**.

## How to Run in Google Colab

To run these notebooks in Google Colab:

1. Go to [Google Colab](https://colab.research.google.com/).
2. Select the **GitHub** tab.
3. Enter the URL of this repository.
4. Click on the notebook you wish to open (`tokenizer.ipynb` or `transformers.ipynb`).
5. Ensure you are using a GPU runtime (**Runtime > Change runtime type > T4 GPU**).

## Running via Visual Studio Code

You can also work with these notebooks directly in VS Code while leveraging Google Colab's free GPU:

1. Open the notebook in VS Code.
2. Ensure you have the **Jupyter** and **Google Colab** extensions installed.
3. Click on the **Kernel Picker** (top right of the notebook editor).
4. Select **Connect to Google Colab**.
5. Follow the authentication prompts to link your Google account.
6. This allows you to run the cells in VS Code while the execution happens on Colab's infrastructure.

You find more details about this integration here - https://developers.googleblog.com/google-colab-is-coming-to-vs-code/

## Notebooks

- **`tokenizer.ipynb`**: Demonstrates the basics of loading the `Phi-3-mini-4k-instruct` model, using the tokenizer to encode prompts, and understanding the input pipeline.
- **`transformers.ipynb`**: Explores more detailed model configuration using `AutoConfig`.

## Setup

Each notebook includes a setup cell to install the necessary libraries directly in your Colab environment:

```python
pip install -U transformers==4.41.2 accelerate==0.31.0 safetensors
```

## Requirements

- A Google account to use Colab.
- A GPU runtime (T4 or better) is recommended for loading and running the Phi-3 model.
