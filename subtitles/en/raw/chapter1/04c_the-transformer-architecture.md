Let's study the transformer architecture. This video is the introductory video to the encoders, decoders, and encoder-decoder series of videos. In this series, we'll try to understand what makes a Transformer network, and we'll try to explain it in simple, high-level terms. No understanding of neural networks is necessary, only an understanding of basic vectors and tensors may help. To get started, we'll take up this diagram from the original transformer paper, entitled "Attention is all you need". As we'll see here we can leverage only some parts of it, according to what we're trying to do. We won't dive into the specific layers building up that architecture, but we'll try to understand the different ways this architecture can be used. Let's first start by splitting that architecture into two parts. On the left we have the encoder, and on the right, the decoder. These two can be used together, but they can also be used independently! Let's understand how these work: The encoder accepts inputs that represent text. It converts this text, these words, into numerical representations. These numerical representations can also be called embeddings, or features.  We'll see that it uses the self-attention mechanism as its main component. We recommend you check out the video on encoders especially to understand what is this numerical representation, as well as how it works. We'll study the self-attention mechanism as well as its bi-directional properties. The decoder is similar to the encoder: it can also accept the same inputs as the encoder: inputs that represent text. It uses a similar mechanism as the encoder, which is the masked self-attention as well. It differs from the encoder due to its uni-directional property, and is traditionally used in an auto-regressive manner. Here too, we recommend you check out the video on decoders especially to understand how all of this works. Combining the two parts results in what is known as an encoder-decoder, or a sequence-to-sequence transformer. The encoder accepts inputs and computes a high-level representation of those inputs. These outputs are then passed to the decoder. The decoder uses the encoder's output alongside other inputs, in order to generate a prediction. It then predicts an output, which it will re-use in future iterations, hence the term "auto-regressive". Finally, to get an understanding of the encoder-decoders as a whole, we recommend you check out the video on encoder-decoders.