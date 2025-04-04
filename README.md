# textforge

textforge takes a plain text file as input, where each line is treated as a single training example, and generates new entries that resemble the originals.

It is an autoregressive character-level language model, offering a range of architectures—from bigrams to modern Transformers (as used in GPT). For example, here I have given a list of company names, textforge can generate original, realistic-sounding business name ideas that match the style and structure of the training data.

This project uses a dataset of ~45,000 company names to train the model.

textforge is lightweight, educational, and designed to be easily hackable. Built with PyTorch, it requires minimal setup and runs on most machines without a GPU.

## Model Architectures

The current implementation includes several model types based on key deep learning papers:

- **Bigram** – One character predicts the next using a lookup table of counts
- **MLP** – Following Bengio et al. (2003)
- **CNN** – Inspired by DeepMind's WaveNet (2016)
- **RNN** – Based on Mikolov et al. (2010)
- **LSTM** – Following Graves et al. (2014)
- **GRU** – From Kyunghyun Cho et al. (2014)
- **Transformer** – Based on Vaswani et al. (2017)
