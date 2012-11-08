test-var
________

| **函数**
| **用途: (test-var v)**

如果 ``v`` 的 ``:test`` 元数据里面有一个函数的话，那么调用这个函数，并且把
``*testing-vars*`` 更新成 ``(conj *testing-vars* v)``

添加于Clojure 1.1
`源码
<https://github.com/clojure/clojure/blob/fa927fd942532fd1340d0e294a823e03c1ca9c89/src/clj/clojure/test.clj#L692>`_
