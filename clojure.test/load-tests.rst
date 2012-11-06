\*load-tests\*
______________
**Var**

默认为true。如果被设置成false的话， ``deftest`` , ``set-test`` 或者 ``with-test`` 就不会产生出任何测试函数。我们可以利用这个来在编译代码的时候忽略测试或者在生产环境加载代码。

在Clojure 1.1里面添加进来的。

`源码
<https://github.com/clojure/clojure/blob/fa927fd942532fd1340d0e294a823e03c1ca9c89/src/clj/clojure/test.clj#L244>`_
