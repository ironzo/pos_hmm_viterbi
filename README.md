# Part of Speech Tagger

This project implements a Part of Speech (POS) Tagger using Hidden Markov Models (HMM) to predict the grammatical parts of speech of words within a given text. The POS tagger is trained on a subset of the Wall Street Journal (WSJ) corpus and can identify various parts of speech, such as nouns, verbs, adjectives, and more.

## Features

- POS tagging using Hidden Markov Models.
- Handling of unknown words using suffix analysis.
- Preprocessing and normalization of text data.
- Evaluation of model accuracy on a test set.

## Installation

Clone this repository to your local machine using:

```bash
git clone https://your-repository-url-here
```

Ensure that you have Python installed, and then install the required Python packages using:

```bash
pip install numpy pandas
```

## Usage

The project can be run from the command line. Navigate to the project directory and execute:

```bash
python part_of_speech.py
```

## Data

The tagger uses two primary datasets:
- `WSJ_02-21.pos`: Training corpus.
- `WSJ_24.pos`: Testing corpus.

These files must be located in the same directory as the script or updated in the script to reflect their path.

## How It Works

The POS tagger processes text to remove punctuation and normalize words, maps words to their respective POS tags, and uses the HMM to predict POS tags for new sentences.

1. **Data Preprocessing:** Prepares the WSJ corpus by removing punctuation and creating a vocabulary of known words.
2. **Model Training:** Trains the HMM on the training corpus to learn transition and emission probabilities.
3. **POS Tagging:** Uses the trained model to predict POS tags for new text inputs.
4. **Evaluation:** Tests the model's accuracy on a separate WSJ test corpus.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your suggested changes.
