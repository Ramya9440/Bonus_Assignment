# Bonus Assignment: Question Answering & Conditional GAN for MNIST Digit Generation

**Student Name:** Ramya Thadikonda  
**Course:** CS5720 - Neural Networks and Deep Learning  
**Submission Type:** Bonus Assignment  
**Total Points:** 1

---

## Task 1: Question Answering with Transformers

### Overview  
Implemented a Question Answering (QA) system using Hugging Face’s `transformers` library with pretrained models.

### What was done  
- Initialized QA pipeline with default model.  
- Switched to a custom pretrained model: `deepset/roberta-base-squad2`.  
- Tested QA on provided and custom contexts with multiple questions.  
- Achieved answers with confidence scores above 0.70.

### How to run  
```bash
pip install transformers torch
python qa_pipeline_default.py
python qa_pipeline_custom_model.py
python qa_custom_context.py
Task 2: Digit-Class Controlled Image Generation with Conditional GAN
Overview
Built a Conditional GAN (cGAN) that generates MNIST digits conditioned on digit class labels (0–9).

What was done
Modified Generator and Discriminator to accept embedded digit labels.

Concatenated label embeddings with noise vectors (Generator input) and image inputs (Discriminator).

Trained on MNIST for 50 epochs.

Saved generated digit images every 10 epochs showing rows of digits conditioned by class.

How to run
bash
Copy
Edit
pip install torch torchvision matplotlib
python training_loop.py
Output
Images saved in generated_images/ folder (e.g., 10.png, 20.png … 50.png) show rows of generated digits, one row per label class.

