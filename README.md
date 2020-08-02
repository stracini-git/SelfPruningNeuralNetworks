# Self-pruning Neural Networks

The connectivity graph of a randomly initialized neural network can be trained directly 
with back-propagation without ever training the actual weights of the network. The link to the
original paper is here: [https://arxiv.org/abs/2006.16627](https://arxiv.org/abs/2006.16627). 
This repository shows how to train a neural network with fixed, random weights, through 
self-pruning layers.

#### How to run
This will run a default experiment: trains a pruning mask for a LeNet-300-100 with fixed weights.
```markdown
python MaskTrainer.py
```

Plot results for the default experiment:
```markdown
python Plotter.py
``` 

