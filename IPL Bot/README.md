Errors I faced 

***AttributeError: type object 'h5py.h5r.Reference' has no attribute '__reduce_cython__'
Makefile:28: recipe for target 'train-nlu' failed
make: *** [train-nlu] Error 1

Solution:  conda install h5py=2.8.0
