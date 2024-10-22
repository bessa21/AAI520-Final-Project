# Overview
This is the final team project for AAI 520 Fall 2024 - Natural Language Processing

Group Members:

Vanessa Laxamana

Nabeel Khan

# Technical Details

This is a chatbot built using the Cornell Movie Dialogs Dataset and implemented in PyTorch. While the bot can engage in conversations and respond to questions, it does not yet pass the Turing Test.

The chatbot is based on a Sequence-to-Sequence (Seq2Seq) architecture with an Attention Mechanism.

The Seq2Seq model, originally introduced in the paper "Learning Phrase Representations using RNN Encoder-Decoder for Statistical Machine Translation," has become a widely used approach for dialogue systems and machine translation. It consists of two Recurrent Neural Networks (RNNs): an encoder and a decoder. The encoder processes a sequence (a sentence) one word at a time, transforming it into a fixed-size feature vector that captures the important information while discarding irrelevant details. Each hidden state depends on the previous one, with the final hidden state summarizing the entire sequence. This final state, often referred to as the "context" or "thought vector," represents the essence of the input. The decoder then uses this context to generate an output sequence, producing one word at a time.

# Dataset 

This corpus contains a large metadata-rich collection of fictional conversations extracted from raw movie scripts:

220,579 conversational exchanges between 10,292 pairs of movie characters

involves 9,035 characters from 617 movies

in total 304,713 utterances

movie metadata included:

genres

release year

IMDB rating

number of IMDB votes

IMDB rating

character metadata included:

gender (for 3,774 characters)

position on movie credits (3,321 characters)

see README.txt (included) for details

The dataset can be downloaded here : Cornell Movie Dialogs Corpus




