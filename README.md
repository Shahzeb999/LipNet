# LipNet
The model architecture used in the research paper "LipNet: End-to-End Sentence-level Lipreading" consists of three main components:

Spatiotemporal convolutional neural network (CNN): This component extracts features from a sequence of video frames of a speaker's mouth. The CNN consists of three layers of 3D convolutions, followed by batch normalization and max pooling layers.

Recurrent neural network (RNN): This component models the temporal dependencies in the sequence of CNN features extracted in the previous step. Specifically, the authors use a bi-directional Gated Recurrent Unit (GRU) layer, which allows the model to capture information from both past and future frames.

Connectionist temporal classification (CTC) layer: This component is used to decode the output of the RNN into a sequence of word probabilities. The CTC layer performs a form of sequence alignment between the output sequence and the ground truth labels, allowing for variable-length outputs.
