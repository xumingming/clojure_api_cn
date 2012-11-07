test-ns
________

| **函数**
| **用途: (test-ns ns)**

如果给定的名字空间里面定义了一个名叫 ``test-ns-hook`` 的函数，那么该函数会调用这个函数。
否则在这个名字空间里面调用 ``test-all-vars`` 。 'ns'参数要么是一个名字空间对象，要么是一个符号。

在该函数的内部会把 ``*report-counters*`` 绑定到一个初始值为
``*inital-report-counters*`` 的ref。并且返回 ``*report-counters*`` 的final的、解引用的值。

添加于Clojure 1.1

`源码
<https://github.com/clojure/clojure/blob/fa927fd942532fd1340d0e294a823e03c1ca9c89/src/clj/clojure/test.clj#L719>`_
