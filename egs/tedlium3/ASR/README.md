
# Introduction

This recipe includes some different ASR models trained with TedLium3.

# Transducers

There are various folders containing the name `transducer` in this folder.
The following table lists the differences among them.

|                        | Encoder   | Decoder            |
|------------------------|-----------|--------------------|
| `transducer_stateless` | Conformer | Embedding + Conv1d |


The decoder in `transducer_stateless` is modified from the paper
[Rnn-Transducer with Stateless Prediction Network](https://ieeexplore.ieee.org/document/9054419/).
We place an additional Conv1d layer right after the input embedding layer.
