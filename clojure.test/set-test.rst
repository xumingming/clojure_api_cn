set-test
________

| **宏**
| **用途: (set-test name & body)**

试验性的。
给这个名为 ``name`` 的var添加一个 ``:test`` 元数据，而这个元数据的值是一个函数，函数体就是传入的 ``body`` 。这个var必须事先存在。这个操作不会改变这个var本身的值。

当 ``*load-tests*`` 为 ``false`` 的时候，``set-test`` 会被忽略掉。

添加于Clojure 1.1

`源码
<https://github.com/clojure/clojure/blob/fa927fd942532fd1340d0e294a823e03c1ca9c89/src/clj/clojure/test.clj#L632>`_
