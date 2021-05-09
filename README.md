# NLP_QuestionAnswer_LSTM

## Dataset Description

Dataset is divided into 17 groupsa and included question - answering pair

## Technique

In this notebook, we use LSTM and BiLSTM to generate answer for the question from user.

LSTM contains 2 processes: train process and inference process. In trainning process, I train the basic LSTM model and save into h5 file. Next, in inference process, I reload the model and define it again

In inference process, there are 2 models which are encode model and decode model. Encode model to collect h_states and c_states in train model, Decode model is used to predict the next word of output sequence

To find the difference, I also defined a model called BiLSTM which basicly the same as LSTM one but It trains into 2 directions which considers to previous states and next states.
