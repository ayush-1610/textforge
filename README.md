# textforge

textforge predicts sequences of characters, specifically predicting the next character in a sequence. It takes a plain text file as input, where each line is treated as a single training example, and generates new entries that resemble the originals.

It is an autoregressive **character-level language model**, offering a range of architectures—from bigrams to modern Transformers (as used in GPT). For example, here I have given a list of company names, textforge can generate original, realistic-sounding business name ideas that match the style and structure of the training data.

#### Bigram Language Model?
A bigram language model predicts the next character in a sequence based on only the preceding character. It works with pairs of characters (bigrams) at a time, looking at a given character and predicting the next. The model is simple and does not capture long-term dependencies between characters.

This project uses a dataset of ~45,000 company names to train the model.
