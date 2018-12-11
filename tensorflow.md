# Tensorflow

## Session
```
a = tf.constant(np.array([1,2,3]))
b = tf.constant(np.array([2,3,4]))
c = tf.add(a,b)
sess = tf.Session()
print(sess.run([a,b,c]))
```

## Basic
* `tf.constant('hello world')`
* `tf.add(a,b) #broadcasts result`
* `tf.placeholder(tf.float32, [None,3])`
* `tf.Variable(tf.random_normal([3,2])) # make a [3,2] array of random normal distribution`
* `sess.run(tf.global_variables_initializer()) # needed to use variables in session`

