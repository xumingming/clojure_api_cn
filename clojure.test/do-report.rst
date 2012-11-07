do-report
_________

| **函数**
| **用途: (do-report m)**

把文件和行号信息添加到测试结果里面去，然后调用 ``report`` 。如果你要写一个自定义的 ``assert-expr`` 方法的话，那么调用这个函数来把测试结果传给 ``report``。
添加于Clojure 1.2。
