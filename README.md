# Self-pruning Neural Networks

The connectivity graph of a randomly initialized neural network can be trained directly 
with back-propagation without ever training the actual weights of the network. The link to the
original paper is here: [https://arxiv.org/abs/2006.16627](https://arxiv.org/abs/2006.16627). 
This repository shows how to train a neural network with fixed, random weights, through 
self-pruning layers. These networks are used here for doing image classification on MNIST
and CIFAR.

#### How to run
This will run a default experiment: trains a pruning mask for a LeNet-300-100 with fixed weights on MNIST.
```markdown
python trainer.py
```

Plot results for the default experiment:
```markdown
python plotter.py
``` 

Command with all options:
```markdown
python trainer.py --outputpath Outputs --trainweights False --trainmasks True --nettype LeNet --p1 0.5 --alpha 0 --masktype mask --activation relu --initializer he --lr 0.001 --batchsize 25 --maxepochs 5 --seed 1234
``` 