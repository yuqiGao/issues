## tensor2tensor
## tensorflow
##### Could not load dynamic library 'libcudart.so.10.1'; dlerror: libcudart.so.1: cannot open shared object file: No such file or directory
Solved: conda install cudatoolkit=10.1

## tensorflow-hub
##### RuntimeError: Exporting/importing meta graphs is not supported when eager execution is enabled. No graph exists when eager execution is enabled.
##### tf.placeholder() is not compatible with eager execution
##### TypeError: 'AutoTrackable' object is not callable
Solving A: [check version of tensorflow:Can a TensorFlow Hub module be used in TensorFlow 2.0?](https://stackoverflow.com/questions/55585079/can-a-tensorflow-hub-module-be-used-in-tensorflow-2-0)

Solving B: [tf.placeholder() is not compatible with eager execution](https://blog.csdn.net/weixin_43763859/article/details/104537392)

Solving C: [Load tf1 model with tf2 in hub: Offical Q&A](https://www.tensorflow.org/hub/common_issues) [Offical moving tf1 to tf2](https://www.tensorflow.org/hub/migration_tf2)
