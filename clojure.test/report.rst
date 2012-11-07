report
______

| **var**

这是一个通用的报告函数，可以被重写成不同的报告格式(比如TAP， JUnit)。像 ``is`` 之类的函数会调用 ``report`` 来显示测试结果。被传给 ``report`` 的参数是一个包含有 ``:type`` 的map。可以通过查看 ``test_is.clj`` 文件的最上面详细看看传给这个函数的 ``:type`` 。

添加于Clojure 1.1

`源码
<https://github.com/clojure/clojure/blob/fa927fd942532fd1340d0e294a823e03c1ca9c89/src/clj/clojure/test.clj#L324>`_
