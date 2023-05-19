# What is a Vision Transformer?

![image](full vision transformer image)

For answering this question we first need to know what is a Transformer?
The transformer was created by Vaswani(2017 Attention is all you need) the 
transformer is a deep learning model that uses the mechanisms of attention
to mesure the relevance of a vector among the other´s vector that compose the input (fig 2), it was created not for vision tasks but for natural lenguage processing(nlp).

![image](attention in transformers), 

![image](encoder decoder)

The Transformer archicture is divide in two big parts, encoder and decoder, both are stack`s of transformer's blocks. A transformer block is a conjunction of layers and other matemathical operations, before diving into them, some cocenpts are important to learn.

### Key concepts: 

- Layer Normalize (LayerNorm)
- Feedforward Layer
- Residual connection
- Self-attention
- Softmax
- pretaining

!!!!!!!!!
Explicar cada uno y ahi avanzar hacia aca..
!!!!!!!!!

### Mathematical concepts:
- Tensor: As like a vector, but with multi-dimension, acctualy it's more general tham a vector or a matrix, both can be represented as a tensor of dimension 1 and 2 respectively, it`s a representation of a space coordinates.

- Linear Projection: Maps vectors from one space to another in a linear manner. It can be used to reduce the dimensionality of data while retaining essential information
(cito chat gpt? xD ayuda )

## Transformer Blocks:
![image](Transformer Block)

"The self-attention calculation lies at the core of what’s called a transformer block,
which, in addition to the self-attention layer, includes additional feedforward layers, residual connections, and normalizing layers."(https://web.stanford.edu/~jurafsky/slp3/10.pdf page 6 10.1.1 Transformer Blocks). Here the input and output dimensions are matched !!!!!(this way the can be stacked permitting more parallelism).

### Attention
...

### Self-Attention
...

## Encoder-Decoder

...

## Traning vs Prediction

...

## ViT (Vision in Transformer) Finally

...

### Image Patches

...

## Understanding Hyperparameters

...

## State-of-Art in ViT

...

## For nerds

### Algorithm Complexity

...

Read more at: https://viso.ai/deep-learning/vision-transformer-vit/