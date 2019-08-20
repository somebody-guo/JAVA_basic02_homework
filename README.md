# JAVA_basic02_homework
### 1. Why should you have minimum scope for variables?  
减小变量的作用域可以增加变量的可控性，减少因变量被非正常修改的可能性与所造成的影响，同时增加代码的可读性与可维护性。  
### 2.Why should you understand performance of String Concatenation?
JAVA的String对象是不可变对象，其值不允许修改，每次通过+或concat进行字符串拼接时都会分配新的对象，这个过程消耗了大量资源，应该用StringBuilder与StringBuffer来替代。
### 3.What are the best practices with Exception Handling?
1) 为可恢复的错误使用检查型异常，为编程错误使用非检查型错误
2) 在finally程序块中关闭或者释放资源
3) 在堆栈跟踪中包含引起异常的原因
4) 始终提供关于异常的有意义的完整的信息
5) 避免过度使用检查型异常
6) 将检查型异常转为运行时异常
7) 记住对性能而言，异常代价高昂
8) 避免catch块为空
9) 使用标准异常
10) 记录任何方法抛出的异常
### 4. When is it recommended to prefer Unchecked Exceptions?
为不可恢复的错误使用非检查型异常
对于无法预知类型的错误使用非检查异常
### 5.When do you use a Marker Interface?
编程语言本身不支持为类维护元数据。而标记接口则弥补了这个功能上的缺失——一个类实现某个没有任何方法的标记接口，实际上标记接口从某种意义上说就成为了这个类的元数据之一。运行时，通过编程语言的反射机制，我们就可以在代码里拿到这种元数据。
### 6.Why are ENUMS important for Readable Code?
从语义的角度使用户可以更方便地在使用常量时展示常量的含义
### 7. Why should you minimize mutability?
1) 不可变的对象线程安全，让并发编程变得更简单  
2) 消除副作用，减小维护成本  
3) 减少容器使用过程出错的概率，例如hashMap的key  
### 8. What is functional programming?
函数式编程是一种编程范式。它把计算当成是数学函数的求值，从而避免改变状态和使用可变数据。它是一种声明式的编程范式，通过表达式和声明而不是语句来编程。
一个函数的输出由且仅由其输入决定，同样的输入永远会产生同样的输出。这使得函数式编程在处理很多与状态相关的问题时，函数式编程的代码通常更加简洁。
### 9. Why should you prefer Builder Pattern to build complex objects?
复杂对象构造时拥有众多参数，可读性差，builder pattern使用链式调用，一步一步的把对象构建出来，使得整个构造过程更加清晰。
### 10. Why should you avoid floats for Calculations?
浮点型数据存储方式导致浮点数的计算在精度上会有损失，一旦这种误差带来程序错误是很难发现的。
### 11. Why should you build the riskiest high priority features first?
降低高风险功能在项目后期引起蝴蝶效应的风险
