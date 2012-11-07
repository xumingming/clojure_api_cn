file-position
_____________

| **函数**
| **用途: (file-position n)**
返回堆栈上的第 ``n`` 个调用，返回的是一个vector: ``[filename line-number]`` 。

在Clojure 1.2里面被废弃掉了: 这个文件和行号信息现在在结果map里面的 ``:file`` 和 ``line`` 上面了。
添加与Clojure 1.1
废弃于Clojure 1.2

