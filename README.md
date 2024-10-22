# Overview
This is the final team project for AAI 520 Fall 2024 - Natural Language Processing

Group Members:

Vanessa Laxamana

Nabeel Khan

# Technical Details

This is a chatbot built using the Cornell Movie Dialogs Dataset and implemented in PyTorch. The bot can engage in conversations and answer user questions, but it does not yet pass the Turing Test.

The chatbot is based on a hybrid approach that combines a Sequence-to-Sequence (Seq2Seq) architecture with an Attention Mechanism and the GPT-2 language model, allowing it to generate both structured responses and free-form conversations. Additionally, the bot includes a set of predefined responses to handle common greetings and questions.

Sequence-to-Sequence (Seq2Seq) Model with Attention:
The Seq2Seq model, originally introduced in the paper "Learning Phrase Representations using RNN Encoder-Decoder for Statistical Machine Translation," is a widely used approach for dialogue systems and machine translation. It consists of two Recurrent Neural Networks (RNNs): an encoder and a decoder. The encoder processes an input sequence (a sentence) one word at a time, transforming it into a fixed-size feature vector that captures the important information while discarding irrelevant details. The final hidden state, also known as the "context" or "thought vector," summarizes the input sequence. The decoder then uses this context to generate an output sequence, producing one word at a time. Attention mechanism allows the model to focus on specific parts of the input when generating each word in the output, improving response relevance.

GPT-2 for Free-Form Conversations:
To enhance the chatbot’s ability to handle more open-ended conversations, the GPT-2 model is integrated. GPT-2 is a powerful pre-trained language model capable of generating human-like text based on a given input prompt. It is particularly useful for generating responses in situations where the input is too complex for the Seq2Seq model or when the conversation is less structured. GPT-2 uses a conversation history to maintain context over multiple exchanges.

Predefined Responses:
For handling common user inputs like greetings or frequently asked questions, predefined responses are included. This allows the chatbot to respond immediately to simple inputs such as "hello" or "what is your name?" without invoking the Seq2Seq or GPT-2 models.

Hybrid Response Generation:
Short or Simple Inputs: The Seq2Seq model with attention is used for handling shorter, more structured queries.
Complex or Free-Form Inputs: For longer, more complex queries or conversational inputs, the GPT-2 model generates responses.
Predefined Responses: For specific predefined queries like "hello" or "how are you?", the chatbot responds from a set of predefined answers.
This hybrid approach allows the chatbot to balance structured dialogue generation with the flexibility of open-ended conversation, creating a more versatile interaction experience.

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




