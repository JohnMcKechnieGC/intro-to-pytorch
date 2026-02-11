# PyTorch Demo
This PyTorch demo is based around some of the ideas we encountered when looking at the browser-based [TensorFlow playground](https://playground.tensorflow.org/).

The pre-trained neural network for image classification demo is adapted from chapter 2 of Deep Learning with PyTorch by Thomas Viehmann, Eli Stevens, Luca Pietro Giovanni Antiga, Manning Publications. The original code is available from the book's [GitHub repo](https://github.com/deep-learning-with-pytorch/dlwpt-code/blob/master/p1ch2/2_pre_trained_networks.ipynb).

In class we also saw a couple of reference implementations from the [PyTorch Pocket Reference](http://pytorchbook.com) book by [Joe Papa](http://joepapa.ai); content is available [on GitHub](https://github.com/joe-papa/pytorch-book).

## Dependencies
You will need to the following to run these notebooks:
pandas
seaborn
ipykernel

You will also need torch and torchvision. You have some options on how to install these.

In my case, I have a compatible NVIDIA GPU, so I configured my environment to use that. You don't need to use a GPU with the examples in this project. Even if you have a compatible GPU, selecting CPU is simpler and fine for these demos, but you might see a significant performance hit when training larger models with more data.

To install PyTorch use https://pytorch.org/get-started/locally/ to generate the right pip install command for your system. In my case, I selected CUDA 13.0 and copied the following command from the webpage:
pip3 install torch torchvision --index-url https://download.pytorch.org/whl/cu130

You will need to make sure you select the right operating system and compute platform for your system.

I next updated my graphics driver to ensure that it was compatible with my system and that it supported the version of CUDA that PyTorch was built with (13.0 in my case):
https://www.nvidia.com/en-gb/drivers/
