#Sentence Autocomplete with Bi-LSTM & GloVe
This project is a deep learning-based Next Word Predictor trained on Medium article titles. It suggests the most likely word to follow a given phrase using a Bidirectional LSTM and pre-trained GloVe word embeddings.

✨ Features
Predictive Text: Generates natural-sounding continuations for sentences.

Bi-LSTM Architecture: Processes text in both directions (forward and backward) to capture a deeper understanding of sentence context.

Transfer Learning: Leverages 100-dimensional GloVe vectors for a rich, pre-trained vocabulary.

Custom Creativity: Includes Temperature-based sampling to control whether predictions are predictable or creative.

🏗️ Project Structure
autocomplete_trainer.py: The single script containing data loading, training, and prediction logic.

tokenizer.pkl: Saved word index for consistent predictions.

autocomplete_model.h5: The trained neural network weights.

🚀 Setup & Usage
1. Requirements
Install the necessary Python libraries:

Bash

pip install tensorflow numpy pandas scikit-learn
2. External Files
To run this project, you need to place the following files in the project root:

medium.csv: The dataset containing article titles (ensure the column is named title).

glove.6B.100d.txt: Pre-trained vectors from Stanford NLP.

3. Run
Execute the main script to clean data, train the model, and enter the interactive testing mode:

Bash

python autocomplete_trainer.py
📂 Exported Files
Upon completion, the script automatically saves the following files for future use:

autocomplete_model.h5

tokenizer.pkl
Note on File Management
This repository includes a .gitignore file to ensure that large data files (like the GloVe vectors and the dataset) are not accidentally uploaded to GitHub. This keeps the repository lightweight and focused on the source code.
