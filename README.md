Bonus Assignment: Question Answering & Conditional GAN for MNIST Digit Generation

Student Name: Ramya Thadikonda
Course: CS5720 - Neural Networks and Deep Learning
Submission Type: Bonus Assignment
Total Points: 1

------------------------------------------------------------
Task 1: Question Answering with Transformers
------------------------------------------------------------

Overview:
Implemented a Question Answering (QA) system using Hugging Face’s transformers library with pretrained models.

What was done:
- Used the default QA model pipeline.
- Switched to a custom model: deepset/roberta-base-squad2.
- Tested QA on both given and self-created contexts.
- Achieved high-confidence answers (>0.70 score).

How to run:
1. Install dependencies:
   pip install transformers torch

2. Run the scripts:
   python qa_pipeline_default.py
   python qa_pipeline_custom_model.py
   python qa_custom_context.py

------------------------------------------------------------
Task 2: Digit-Class Controlled Image Generation with Conditional GAN
------------------------------------------------------------

Overview:
Built a Conditional GAN (cGAN) that generates MNIST digit images based on label inputs (0 to 9).

What was done:
- Modified Generator and Discriminator to take digit labels as input.
- Embedded class labels and concatenated with noise/image vectors.
- Trained the cGAN for 50 epochs using the



