## tensor2tensor
##### ImportError: cannot import name 'contrib'/AttributeError: module 'tensorflow' has no attribute 'contrib'
Temp solve: Just comment it and ignore
##### grid_lip never registered with registry env_problems.
Solved: Need to specify t2t_usr_dir
#####  TypeError: Input 'y' of 'Sub' Op has type float32 that does not match type int32 of argument 'x'.
Solved: Might be caused by the problem generate wrong samples.

## tensorflow 
##### Could not load dynamic library 'libcudart.so.10.1'; dlerror: libcudart.so.1: cannot open shared object file: No such file or directory
Solved: conda install cudatoolkit=10.1
##### Could not load dynamic library 'libcudart.so.10.0'; dlerror: libcudart.so.10.0: cannot open shared object file: No such file or directory
Solved: conda install cudatoolkit=10.0
##### Could not load dynamic library 'libcudnn.so.7'; dlerror: libcudnn.so.7: cannot open shared object file: No such file or directory; LD_LIBRARY_PATH: /usr/local/cuda/lib64:/share/local/slocal/lib:/usr/local/cuda/lib64:/share/local/lib:$LD_LIBRARY_PATH
Not solve: conda install cudnn
Solved: conda install -c anaconda cudnn
##### ERROR: Cannot uninstall 'wrapt'. It is a distutils installed project and thus we cannot accurately determine which files belong to it which would lead to only a partial uninstall.
Solved: pip install -U --ignore-installed wrapt enum34 simplejson netaddr [csdn](https://www.cnblogs.com/xiaowei2092/p/11025155.html)
##### ModuleNotFoundError: No module named 'tensorflow.compat'
Solved: upgrade tensorflow

##### Unable to Enable Tensorflows Eager execution: AttributeError: module 'tensorflow' has no attribute 'enable_eager_execution'
Solved: tf.enable_eager_execution() in tensorflow 1.x, in tensorflow 2, eager mode is set to be open default.
##### 

## tensorflow-hub
##### RuntimeError: Exporting/importing meta graphs is not supported when eager execution is enabled. No graph exists when eager execution is enabled.
##### tf.placeholder() is not compatible with eager execution
##### TypeError: 'AutoTrackable' object is not callable
Solving A: [check version of tensorflow:Can a TensorFlow Hub module be used in TensorFlow 2.0?](https://stackoverflow.com/questions/55585079/can-a-tensorflow-hub-module-be-used-in-tensorflow-2-0)

Solving B: [tf.placeholder() is not compatible with eager execution](https://blog.csdn.net/weixin_43763859/article/details/104537392)

Solving C: [Load tf1 model with tf2 in hub: Offical Q&A](https://www.tensorflow.org/hub/common_issues) [Offical moving tf1 to tf2](https://www.tensorflow.org/hub/migration_tf2)
