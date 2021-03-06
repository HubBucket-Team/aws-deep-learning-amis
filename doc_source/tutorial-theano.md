# Theano<a name="tutorial-theano"></a>

## Theano Tutorial<a name="tutorial-theano-overview"></a>

To activate the framework, follow these instructions on your Deep Learning AMI with Conda\.

For Theano \+ Keras in Python 3 with CUDA 9 with cuDNN 7:

```
$ source activate theano_p36
```

For Theano \+ Keras in Python 2 with CUDA 9 with cuDNN 7:

```
$ source activate theano_p27
```

Start the iPython terminal\.

```
(theano_p36)$ ipython
```

Run a quick Theano program\.

```
import numpy
import theano
import theano.tensor as T
from theano import pp
x = T.dscalar('x')
y = x ** 2
gy = T.grad(y, x)
pp(gy)
```

You should see Theano computing a symbolic gradient\.

## More Tutorials<a name="tutorial-theano-more"></a>

For further tutorials and examples refer to the framework's official docs, [Theano Python API](http://deeplearning.net/software/theano/library/index.html), and the [Theano](http://deeplearning.net/software/theano/) website\.