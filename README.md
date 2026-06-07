# E-Commerce Chatbot using Large Language Model (LLM)

## Project Overview

This project focuses on building an AI-powered E-Commerce Chatbot using a Large Language Model (LLM). The chatbot is trained on product information from a Flipkart e-commerce dataset and can answer customer queries related to products, brands, descriptions, and pricing.

The project demonstrates the complete workflow of developing a domain-specific chatbot, including data preprocessing, dataset creation, model fine-tuning, testing, and deployment through a Gradio web interface.

---

## Features

- Product Question & Answer chatbot
- Fine-tuned DistilGPT2 model
- Automatic Q&A dataset generation
- Hugging Face Transformers integration
- Gradio-based user interface
- Product information retrieval
- Price and brand query support

---

## Dataset

The project uses a Flipkart E-Commerce Dataset containing:

- Product Name
- Description
- Brand
- Retail Price
- Discounted Price
- Additional product information

Dataset Size:

- 3000 products
- 6 columns

---

## Technologies Used

- Python
- Pandas
- Hugging Face Transformers
- Hugging Face Datasets
- DistilGPT2
- Gradio
- Google Colab

---

## Project Workflow

### 1. Data Loading
- Load Flipkart product dataset
- Handle missing values
- Explore dataset structure

### 2. Q&A Dataset Creation
Generate multiple question-answer pairs for each product:

Examples:

**Question:** What is this product?

**Answer:** Product description

**Question:** Which brand makes this product?

**Answer:** Brand name

**Question:** What is the retail price?

**Answer:** Product retail price

**Question:** What is the discounted price?

**Answer:** Product discounted price

---

### 3. Model Selection

Pre-trained model used:

```python
distilgpt2
```

DistilGPT2 was selected because it is:

- Lightweight
- Faster to train
- Suitable for educational projects
- Easy to fine-tune

---

### 4. Tokenization

The generated Q&A dataset is tokenized using the Hugging Face tokenizer.

Configuration:

- Maximum Length: 64
- Padding: Max Length
- Truncation: Enabled

---

### 5. Model Training

Training Configuration:

| Parameter | Value |
|------------|---------|
| Epochs | 3 |
| Batch Size | 8 |
| Model | DistilGPT2 |
| FP16 | Enabled |
| Save Checkpoints | Limited |

The model learns to generate answers based on product-related questions.

---

### 6. Model Testing

Sample Query:

```text
Question: Which brand makes a product?
```

The chatbot generates responses based on the knowledge learned during training.

---

### 7. Deployment with Gradio

A Gradio interface is created for user interaction.

Features:

- Simple web interface
- Real-time chatbot responses
- Easy deployment
- User-friendly experience

---

## Installation

Install required libraries:

```bash
pip install transformers datasets accelerate gradio pandas
```

---

## Running the Project

### Step 1: Clone Repository

```bash
git clone <repository-url>
```

### Step 2: Install Dependencies

```bash
pip install transformers datasets accelerate gradio pandas
```

### Step 3: Run Notebook

Open and execute:

```text
LLM_ecommerce_chatbot.ipynb
```

### Step 4: Launch Chatbot

Run the Gradio section to start the chatbot interface.

---

## Sample Questions

Try asking:

- What is this product?
- Which brand makes this product?
- What is the retail price?
- What is the discounted price?
- Give details about this product.

---

## Results

- Successfully generated a custom Q&A dataset.
- Fine-tuned DistilGPT2 on e-commerce product information.
- Built an interactive chatbot.
- Deployed the chatbot using Gradio.
- Achieved relevant responses for product-related queries.

---

## Future Improvements

- Use larger LLMs such as GPT-Neo or LLaMA.
- Add Retrieval-Augmented Generation (RAG).
- Support order tracking.
- Add multilingual support.
- Deploy on cloud platforms.
- Improve response accuracy using larger datasets.

---

## Conclusion

This project demonstrates the development of a domain-specific E-Commerce Chatbot using Large Language Models. By combining data preprocessing, automatic Q&A generation, model fine-tuning, and Gradio deployment, the chatbot can provide intelligent responses to customer product-related questions and serve as a foundation for more advanced retail AI assistants.

---

## Author

Akansha Kachhawe

Capstone Project – E-Commerce Chatbot using Large Language Models (LLM)
