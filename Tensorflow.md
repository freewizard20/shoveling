# Tensorflow

## Session
```
a = tf.constant(np.array([1,2,3]))
b = tf.constant(np.array([2,3,4]))
c = tf.add(a,b)
sess = tf.Session()
print(sess.run([a,b,c]))
```
* sess.run을 해야지 값을 채워넣어서 숫자값을 보여주지, 아니면 그냥 빈 골판지 Tensor 오브젝트이다.

## Basic
* `tf.constant('hello world')`
* `tf.add(a,b) #broadcasts result`
* `tf.placeholder(tf.float32, [None,3]) # sess.run(out,feed_dict={X:x_data}) can feed any size if size omitted`
* `tf.Variable(tf.random_normal([3,2])) # make a [3,2] array of random normal distribution`
* `sess.run(tf.global_variables_initializer()) # needed to use variables in session`
* `tf.reduce_mean(tf.square(hypothesis-Y)) # reduce_mean reduces dim by meaning`
