# Theano Short Demo

Purpose of this repo is to demonstrate the fundamentals of Theano. The codes in this repo aims to be clear and contructed from the bottom.

## Dependency
* __Theano (numpy)__: Of course you need `Theano`. To install it, follow the instruction [here](http://deeplearning.net/software/theano/install.html). `numpy` will be installed alongside.
* __h5py__: We use HDF5 data format to save and load the datasets. In some demos, you need `h5py` package. You can install it by `pip install h5py` but in case you get some errors and you are using Ubuntu, (I don't know why exactly) you may try `apt-get install python-h5py`.

## IPython tricks
### Interactive view (Deprecated in ipython 4.x.x)
With the help of `matplotlib`, you can visualize the data. Now you might want interactive inspection on the data. For example, you might want to inspect image one by one interactively. You can do this by following code snippet.
```python
from __future__ import print_function
from IPython.html.widgets import interact, interactive, fixed
from IPython.html import widgets

@interact(idx=(0,100))
	def viz_data(idx):
		code_for_visualizing_the_idx_th_data()
```

### Animation
You might want to see an animated view. You can do this using `JSAnimation`. You first download `JSAnimation` from [here](https://github.com/jakevdp/JSAnimation). Unzip it and go in to the directory then type `sudo python setup.py install`. A simple usage example is demonstrated [here](http://nbviewer.ipython.org/github/jakevdp/JSAnimation/blob/master/animation_example.ipynb).





