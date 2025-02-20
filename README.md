# Fine-TuningLLMs
Guide to downloading and fine tuning a LLM, to get better results.

In this project I imported google gemini following their guide to use their model, and acquired an API key to work with. I then read their Fine tuning section for their LLM, and began to work towards optimizing my client of Gemini to produce better results.
There are some things we must know before this:
Google Gemini intro to Tuning:
Advanced tuning settings
When creating a tuning job, you can specify the following advanced settings:

Epochs: A full training pass over the entire training set such that each example has been processed once.
Batch size: The set of examples used in one training iteration. The batch size determines the number of examples in a batch.
Learning rate: A floating-point number that tells the algorithm how strongly to adjust the model parameters on each iteration. For example, a learning rate of 0.3 would adjust weights and biases three times more powerfully than a learning rate of 0.1. High and low learning rates have their own unique trade-offs and should be adjusted based on your use case.
Learning rate multiplier: The rate multiplier modifies the model's original learning rate. A value of 1 uses the original learning rate of the model. Values greater than 1 increase the learning rate and values between 1 and 0 lower the learning rate.

Google Gemini's Default Configuration:
Epoch: 5 Batch size: 4 Learning rate:0.001

