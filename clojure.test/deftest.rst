deftest
_______

|  **宏**
|  **用途: (deftest name & body)**

定义一个无参数的测试函数。测试函数可以调用其它测试函数，所以测试函数是可以组合的。如果你要编写组合测试的话，那么你就一定要编写一个名叫 ``test-ns-hook`` 的函数；``run-test`` 会调用所有的 ``test-ns-hook`` 函数，而不是所有的var。
注意: 实际上，测试代码的主体是保存在var的 ``:test`` 元数据里面的，而真正的函数(这个var的值)对它自己调用 ``test-var`` 。

当 ``*load-tests*`` 为false的时候， ``deftest`` 会被忽略掉。

在Clojure 1.1里面添加的。

::

    ;successful test example
    (ns testing)
    (use 'clojure.test)


    (deftest addition
      (is (= 4 (+ 2 2)))
      (is (= 7 (+ 3 4))))
    => #'testing/addition

    (deftest subtraction
      (is (= 1 (- 4 3)))
      (is (= 3 (- 7 4))))
    => #'testing/subtraction

    ;composing tests
    (deftest arithmetic
      (addition)
      (subtraction))
    => #'testing/arithmetic

    (run-tests 'testing)

    => Testing testing

    Ran 6 tests containing 10 assertions.
    0 failures, 0 errors.
    {:type :summary, :test 6, :pass 10, :fail 0, :error 0}

