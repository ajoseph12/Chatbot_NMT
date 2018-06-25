Cornell Movie Dialog Chatbot
===================


Introduction
-------------

The Cornell Movie Dialog Chatbot is an implementation of a chatbot using NMT - Neural Machine Translation (seq2seq).

The code for the creation of the chatbot has been forked form https://github.com/daniel-kukiela/nmt-chatbot. Once this
was done I had to simply follow the setup instructions to get my chatbot up and running. The chatbot here has been trained 
on the  Cornell Movie Dialog corpus using a laptop with rather modest specs (16 GB ram, 2GB V graphics and 1TB storage).


Parameters
-------------
Following were the values assigned to the parameters/hyperparameters:
- Vocabulary size : 10,000
- Attention mechanism : Bahdanau
- Number of steps : 50,000
- Number of layers : 2
- Number of units : 512
- Optimizer : Adam
- Encoder type : Bi-directional
- Beam width : 10
- Batch size : 128
- Dropout : 0.2


Getting started
-------------

Steps to setup the chatbot are as follows:

1. Download all files in the link ```https://drive.google.com/open?id=1kZQVW3ZWug-GdnN19QXbQazntAkgwQVg``` 
and store it in a folder named 'model'.
2. ```$ git clone https://github.com/ajoseph12/nmt-chatbot.git```
3. Move earlier created folder 'model' into the nmt-chatbot repo.
4. ```$ pip install -r requirements.txt```
5. ```$ cd model```
6. Open the checkpoint file and modify the path to the one where the checkpoint files currently are.
7. Open the hparams file and modify the key values of "src_vocab_file" and "tgt_vocab_file" to the path 
to which each respective file belongs. (\'filepath'\data for scr and tgt vocab )
8. ```$ cd ..```
9. ```$ python modded-inference.py ```

Have fun :)