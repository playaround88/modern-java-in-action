# 关于本书

## 索引
* <a href="#roadmap">本书如何组织:学习路线</a>
* <a href="#code">关于书中源码</a>
* <a href="#forum">本书论坛</a>

<p class="en">Put simply, the new features in Java 8 along with the (less-obvious) changes in Java 9 are the biggest change to Java in the 21 years since Java 1.0 was released. Nothing has been taken away, so all your existing Java code continues to work—but the new features provide powerful new idioms and design patterns to help you write clearer, more concise code. At first you might think (as with all new features), “Why are they changing my language again?” But then, after a bit of practice, comes the revelation that you’ve just used the features to write shorter, clearer code in half the time you expected—and you realize you could never go back to “old Java” again.</p>

简单来说, 在Java 8和Java 9(不明显)引入的新特性是Java自1.0版本发布后21年来最大的变化. 没有任何语法被移除, 所以你所有已有的Java代码可以继续工作-但新特性提供了更有力的用法和设计模式来帮助你编写更干净,更简洁的代码. 一开始你可能认为(与所有的新特性一样), "他们为何有要改变语法?" 但经过一些实践之后, 随着你使用新特性, 使用比预期更少的时间编写了更短,更干净的代码-接着你就会意识到你再也不愿意回到旧版本的Java了.

<p class="en">The second edition of this book, Modern Java in Action: Lambdas, Streams, Functional and Reactive Programming, is written to get you over that initial hump of “sounds good in principle, but it’s all a bit new and unfamiliar” and into coding like a native.</p>

《Modern Java in Action》第二版: Lambdas, Streams, Functional and Reactive Programming, 本书主要是为了帮助你度过开始的障碍"听起来简单, 但总是遇到新的不熟悉的点", 并且使你能够熟悉这样的编程方式.

<p class="en">“Perhaps,” you might think, “but lambdas, functional programming—aren’t those the sort of things that bearded sandal-wearing academics talk about in their ivory towers?” They might be, but Java 8 has incorporated just the right balance of ideas into Java to gain many of their advantages in a way that’s comprehensible to ordinary Java programmers. And this book tells the story from the ordinary-programmer viewpoint, with an occasional “how this arose” for perspective.</p>

也许, 你可能在想, "但lambda, 函数式编程-并不是那些在他们象牙塔的(顶尖的)学术讨论的内容呐?"它们可能是, 但是Java 8以一种普通程序员可以理解的方式, 引入了这些概念来得到了它们的许多优点, 并找到了平衡点. 这本书从普通程序员的角度来讲述故事, 并会不时的展望"周围风景如何?".

<p class="en">“Lambdas—that sounds Greek to me!” Yes, it does, but it’s a great idea for enabling you to write concise Java programs. Many of you are familiar with event handlers and callbacks, where you register an object containing a method to be used when some event happens. Lambdas make this sort of idea much more widely usable in Java. Put simply, lambdas and their friends, method references, provide the ability to concisely pass code or methods as arguments to be executed in the middle of doing something else. You’ll see in this book how this idea occurs more frequently than you might think: from simply parameterizing a sort method with code to do the comparison to expressing complex queries on collections of data using the new Streams API.</p>

"Lambda-对我来说一窍不通"是吗, 也许是, 但是它是你编写简洁代码的一个很好的概念. 很多读者应该都对event handlers和callbacks比较熟悉, 那些需要你注册当事件发生时调用的包含一个方法的对象. Lambdas使这样的概念变的在更广泛范围可用. 简单来说, lambda和它的"朋友", 方法引用, 提供了简洁的把代码和方法作为参数传递到其他执行代码中的能力. 你将会在本书中比你预想的更经常的看到这个概念的出现: 从简单的给排序传递一个比较方法参数, 到表达复杂的使用新的streams API完成数据集合查询. 

<p class="en">“Streams—what are they?” They’re a great new Java 8 addition. They behave like collections but have several advantages that enable new styles of programming. First, if you’ve ever programmed using a database-query language such as SQL, you’ll recognize that it enables queries to be written in a few lines that would take many lines in Java. Java 8 streams support this concise database-queries style of programming— but with Java syntax and none of the need to know about databases! Second, streams are designed so that not all their data needs to be in memory (or even computed) at once. Thus, you can process streams that are too big to fit in your computer memory. But Java 8 can optimize operations on streams in a way that Java can’t do for collections—for example, it can group together several operations on the same stream so that the data is traversed only once instead of expensively traversing it multiple times. Even better, Java can automatically parallelize stream operations for you (unlike collections).</p>

"streams-它们是什么?" 它们是Java 8版本的重要新特性. 它们的行为像集合但是拥有一些新风格编程的优点. 首先, 如果你还没有使用过像SQL的数据库查询语言, 你将会意识到相比Java的多行代码, 它让你可以使用简单几行代码编写查询. Java 8 streams支持这样的简洁的数据库查询风格的编程-使用Java语法, 并且不需要知道数据库的知识! 其次, streams被设计为不需要一次把所有的数据到放到内存中(甚至计算). 因此, 你可以处理那些超过你的内存的非常大量的数据流. 但是Java 8可以以在集合上不可能的方式来优化在streams上的操作-例如, 它可以把同一个streams上的操作分组, 这样数据处理只需要执行一遍, 而不是"昂贵的"执行多遍遍历. 更厉害的是, Java可以自动的为你并发执行流程操作(不像集合).

<p class="en">“And functional-style programming, what’s that?” It’s another style of programming, just like object-oriented programming, but centered on using functions as values, just as we mentioned previously when discussing lambdas.</p>

"那么函数式风格编程, 又是什么呐?" 它是另一种编程风格, 就像面向对象编程, 但是是以函数当作值为中心, 就像我们上面讨论lambda时候提到的.

<p class="en">What’s great about Java 8 is that it incorporates many of the best ideas from functional programming into the familiar Java syntax. The fine design choices enable you to see functional-style programming in Java 8 as an additional set of design patterns and idioms to enable you to write clearer, more concise code in less time. Think of it as having a wider range of weapons in your programming armory.</p>

Java 8的伟大之处就是他在Java语法中吸纳了许多来自函数编程中最好的概念. 这种好的设计选择使你可以在Java 8中看到函数风格编程, 作为一种附加的设计模式和用法使你可以使用更少的时间编写更干净, 更简洁的代码. 可以把他认为你程序兵器谱中多了许多武器.

<p class="en">Oh yes, in addition to these features that lean on big conceptual additions to Java, we also explain the many other useful Java 8 features and updates such as default methods, the new Optional class, CompletableFuture, and the new Date and Time API.</p>

好的, 除了这些Java新增加的大的框架特性, 我们还会解释很多其他的有用的Java 8特性和更新, 例如默认方法, 新的Optinal类, CompletableFuture和新的Date/Time API.

<p class="en">And there are the Java 9 additions: a new module system, support for reactive programming via the Flow API, and various other enhancements.</p>

并且还有一些Java 9的演进: 一个新的模块系统, 通过Flow API支持的响应式编程, 和一些其他的增强.

<p class="en">But hey, this is an overview, and it’s time now for us to leave you to read the book.</p>

但注意, 这只是一个整体预览, 现在对我们来说是时候开始阅读这边书了. 

## <a name="roadmap">本书如何组织:学习路线</a>

<p class="en">Modern Java in Action is divided into six parts: “Fundamentals,” “Functional-style data processing with streams,” “Effective programming with streams and lambdas,” “Everyday Java,” “Enhanced Java concurrency,” and “Functional programming and future Java evolution.” While we strongly recommend that you read the chapters in the first two parts first (and in order because many of the concepts presented build on previous chapters), the remaining four parts can be read reasonably independently. Most chapters include several quizzes to help you work through the material.</p>

Modern Java in Action被分成了六个部分：“起源”，“使用streams函数风格数据处理”，“使用streams和lambda高效开发”，“常用Java”，“增强的Java并发”和“函数式编程和未来Java的演进”。我们强烈建议你首先阅读前面两个部分（顺序阅读，因为很多概念由前面概念引出），剩下的四部分可以适度的独立阅读。大部分章节包含一些测试来帮助你掌握这些资料。

<p class="en">The first part of the book provides the fundamentals to help you get started with the new Java ideas introduced in Java 8. By the end of this first part, you’ll have a full understanding of what lambda expressions are, and you’ll be able to write code that’s both concise and flexible enough to easily adapt to changing requirements.</p>

本书第一部分提供了起源来帮助你了解Java 8引入的新的概念。在学完第一部分后，你将会全面的理解什么是lambda表达式，并且你将会能够编写即简洁又能够灵活适应需求变化的代码。

■ In chapter 1, we summarize the main changes to Java (lambda expressions, method references, streams, and default methods) and set the scene for the book. 

第一章,我们总结Java的主要变化(lambda表达式,方法引用,streams和默认方法),并为本书设定场景.

■ In chapter 2, you’ll learn about behavior parameterization, a softwaredevelopment pattern that Java 8 relies heavily on and is the motivation for lambda expressions. 

第二章,你将会学习行为参数化,一种Java 8主要依赖的软件开发模式,这也是引入lambda表达式的主要动机.

■ Chapter 3 gives a full explanation, with code examples and quizzes at every step, of the concepts of lambda expressions and method references.

第三章,将会给出lambda表达式和方法引用的详细解释,并为每步都提供了样例代码和测验.

<p class="en">The second part of this book is a deep exploration of the new Streams API, which lets you write powerful code that processes a collection of data in a declarative way. By the end of this second part, you’ll have a full understanding of what streams are and how you can use them in your codebase to process a collection of data concisely and efficiently.</p>

本书第二部分深入探讨新的streams API，它使你能够编写声明式处理集合数据的更有力的代码。在完成第二部分后，你将会全面理解什么是streams，如何在你的代码库中使用它们来更简洁高效的处理集合数据。

■ Chapter 4 introduces the concept of a stream and explains how it compares with a collection.

第4章, 介绍stream的概念以及和现有集合类的对比.

■ Chapter 5 investigates in detail the stream operations available to express sophisticated data-processing queries. You’ll look at many patterns such as filtering, slicing, finding, matching, mapping, and reducing. 

第5章, 审查stream用来处理数据查询的操作. 你将会看到许多模式,例如filtering, slicing, finding, matching, mapping和reducing.

■ Chapter 6 covers collectors—a feature of the Streams API that lets you express even more complex data-processing queries. 

第6章, 覆盖收集器-streams API的一个使你可以表达更加复杂数据处理查询的特性.

■ In chapter 7, you’ll learn about how streams can automatically run in parallel and leverage your multicore architectures. In addition, you’ll learn about various pitfalls to avoid when using parallel streams correctly and effectively.

第7章, 你将学习streams是如何自动并行运行充分使用多核处理器架构. 另外, 你将学习一些正确有效使用streams的方式来避免潜在的风险.

<p class="en">The third part of this book explores various Java 8 and Java 9 topics that will make you more effective at using Java and will enhance your codebase with modern idioms. Because it is oriented toward more-advanced programming ideas we have arranged, nothing later in the book depends on the techniques described here.</p>

本书的第三部分探究Java 8和Java 9引入的那些，使你能够更高效使用Java和你是的代码更符合现代Java用法的主题。因为这些是我们安排的面向高级编程的概念，本书后面的部分并不依赖这里描述的技术。

■ Chapter 8 is a new chapter for the second edition and explores the Collection API Enhancements of Java 8 and Java 9. It covers using collection factories and learning new idiomatic patterns to work with List and Set collections along with idiomatic patterns involving Map. 

第8章, 是第二版的新章节, 探究Java 8和Java 9对集合API的增强, 覆盖了List和Set的集合工厂和新的惯用法, 也包含了Map的惯用模式.

■ Chapter 9 explores how you can improve your existing code using new Java 8 features and a few recipes. In addition, it explores vital software-development techniques such as design patterns, refactoring, testing, and debugging. 

第9章, 探究如何使用新的Java 8特性来改善你的代码库和一些小技巧. 另外, 它探索了极为重要的编程技术, 例如编程模式, 重构, 测试和调试.

■ Chapter 10 is also new for the second edition. It explores the idea of basing an API on a domain-specific language (DSL). This is not only a powerful way of designing APIs but one which is both becoming increasingly popular and is already appearing in the Java classes such as Comparators, Stream, and Collectors.

第10章, 也是第二版新增的章节. 本章探究编写领域语言(domain-specific language)的概念. 这不仅是一个设计API的有利手段同时在Java中已经常见并且越来越流行, 例如在Comparator, stream和Collector接口.

<p class="en">The fourth part of this book explores various new features in Java 8 and Java 9 centered around making it easier and more reliable to code your projects. We start with two APIs introduced in Java 8.</p>

本书的第四部分探讨Java 8和Java 9引入的一些聚焦于易用和可靠性的新特性。我们以Java 8引入的两部分API开始。

■ Chapter 11 covers the java.util.Optional class, which allows you to both design better APIs and reduce null pointer exceptions. 

第11章, 覆盖java.util.Optional类, 它允许你设计更好的API, 并减少空指针异常.

■ Chapter 12 explores the Date and Time API, which greatly improves the previous error-prone APIs for working with dates and time. 

第12章, 探究Date和Time API, 这些API极大的改进了上一版本的Date和time相关的极易出错的API. 然后, 我们探究Java 8和Java 9为编写大型系统和简化演进而加入的增强.

■ In chapter 13, you’ll learn what default methods are, how you can use them to evolve APIs in a compatible way, some practical usage patterns, and rules for using default methods effectively. 

第13章, 你将学习什么是默认方法, 如何使用它们以兼容的方式演进你的API, 一些实践模式, 和使用默认方法的有效规则.

■ Chapter 14 is new for this second edition and explores the Java Module System—a major enhancement in Java 9 that enables huge systems to be modularized in a documented and enforceable way, rather than being “just a haphazard collection of packages.”

第14章, 是第二版新增的章节, 探究Java的模块系统-Java 9版本的一个主要增强, 它使巨型系统通过文档和强制方式来实现模块化, 而不是"可能的包的集合"

<p class="en">The fifth part of this book explores the more advanced ways of structuring concurrent programs in Java—beyond the ideas of easy-to-use parallel processing for streams introduced in chapters 6 and 7. Chapter 15 is new to this second edition and covers the “big-picture” idea of asynchronous APIs—including the ideas of Futures and the Publish-Subscribe protocol behind Reactive Programming and encapsulated in the Java 9 Flow API.</p>

本书的第五部分探讨Java构造并发程序的更高级的方式-不仅是第6、7章介绍的易用的并发streams概念。第15章是本书第二版新增章节，展示异步API的概念全貌, 包括Futrue的概念, 响应式编程和Java 9 Flow API背后的发布订阅协议.

■ Chapter 16 explores CompletableFuture, which lets you express complex asynchronous computations in a declarative way—paralleling the design of the Streams API. 

第16章, 探究CompletableFuture, 它可以用来声明式并发来表达更加复杂的异步计算-Stream API的设计.

■ Chapter 17 is again new to this second edition and explores the Java 9 Flow API in detail, focusing on practical reactive programming code.

第17章, 也是第二版新增的章节, 探究Java 9的Flow API的细节, 聚焦响应式编码的实践.

<p class="en">In the sixth and final part of this book, we draw back a little with a tutorial introduction to writing effective functional-style programs in Java, along with a comparison of Java 8 features with those of Scala.</p>

在本书第六也是最后部分， 我们通过一个书写高效的函数风格的编程指导来做一下简单回顾, 并会简单对比一下Java 8的特性和Scala语言的对比.

■ Chapter 18 gives a full tutorial on functional programming, introduces some of its terminology, and explains how to write functional-style programs in Java. 

第18章, 给出了一个函数编程的完整指导, 介绍了一些术语, 并介绍了如何在Java中编写函数风格的程序.

■ Chapter 19 covers more advanced functional programming techniques including higher-order functions, currying persistent data structures, lazy lists, and pattern matching. You can view this chapter as a mix of practical techniques to apply in your codebase as well as academic information that will make you a more knowledgeable programmer. 

第19章, 覆盖了更高级的函数编程技术包括高阶函数, 柯里化, 持久化数据结构, 延迟列表和模式匹配. 你可以把本章看成使你变成一个更专业的代码实践和理论信息的一个结合章节.

■ Chapter 20 follows by discussing how Java 8 features compare to features in the Scala language—a language that, like Java, is implemented on top of the JVM and that has evolved quickly to threaten some aspects of Java’s niche in the programming language ecosystem.

第20章, 讨论Java 8特性和Scal语言特性的对比, scala是一门类Java的, 在JVM上实现的快速演进的语言, 在某些方面它甚至已经威胁到了Java在编程语言生态中的地位.

■ In chapter 21, we review the journey of learning about Java 8 and the gentle push toward functional-style programming. In addition, we speculate on what future enhancements and great new features may be in Java’s pipeline beyond Java 8, Java 9, and the small additions in Java 10.

第21章, 回顾整个Java 8的学习旅程, 并阐述函数式编程. 另外, 我们推测一些那些特性增强和大的新特性可能会再Java 8/9的后续版本中引入, 以及Java 10的小的变动.

<p class="en">Finally, there are four appendixes, which cover a number of other topics related to Java 8. Appendix A summarizes minor Java 8 language features that we didn’t discuss in the book. Appendix B gives an overview of other main additions to the Java library that you may find useful. Appendix C is a continuation of part 2 and looks at advanced uses of streams. Appendix D explores how the Java compiler implements lambda expressions behind the scenes.</p>

最后，有四个附录部分，他们涵盖了一些Java 8的其他主题。 附录A总结Java 8中我们本书没有讨论的小的特性。附录B给出了其他对你有用的Java工具包的新增内容的主要概览。附录C是本书第二部分的继续，并展示了streams的高级用法。附录D探讨Java编译器背后是如何实现lambda表达式。

## <a name="code">关于书中源码</a>
<p class="en">All source code in listings or in text is in **a fixed-width font like this** to separate it from ordinary text. Code annotations accompany many of the listings, highlighting important concepts. </p>

所有的表或者文本中的源码都是**像这里一样有固定宽度的字符** 以区别与普通文本. 代码声明附和一些表, 用来高亮一些重要概念. 

<p class="en">Source code for all the working examples in the book and instructions to run them are available on a GitHub repository and as a download via the book’s website. Both links to the source code may be found at [www.manning.com/books/modernjava-in-action](http://www.manning.com/books/modernjava-in-action).</p>

本书中所有可运行样例的源码和运行它们的命令，作为本书的下载都可以在GitHub仓库找到。源码和连接都可以在[www.manning.com/books/modernjava-in-action](http://www.manning.com/books/modernjava-in-action)找到。

## <a name="">本书论坛</a>
<p class="en">Purchase of Modern Java in Action includes free access to a private web forum run by Manning Publications where you can make comments about the book, ask technical questions, and receive help from the authors and from other users. To access the forum, go to https://forums.manning.com/forums/modern-java-in-action. You can also learn more about Manning’s forums and the rules of conduct at https://forums .manning.com/forums/about.</p>

购买本书会包含一个免费的登录Manning出版社维护的私有论坛的账户，论坛里可以评论本书的，咨询技术问题，并收到作者或者其他读者的回复。登录论坛，请访问https://forums.manning.com/forums/modern-java-in-action。你可以在下面的网址了解更多关于论坛和引导规则https://forums .manning.com/forums/about。

<p class="en">Manning’s commitment to our readers is to provide a venue where a meaningful dialogue between individual readers and between readers and the authors can take place. It is not a commitment to any specific amount of participation on the part of the authors, whose contribution to the forum remains voluntary (and unpaid). We suggest you try asking the authors some challenging questions lest their interest stray! The forum and the archives of previous discussions will be accessible from the publisher’s website as long as the book is in print.</p>

Manning出版社对我们的读者承诺会提供一个可以在读者之间或者读者与作者直接可以进行有意义对话的地方。 但这不是对作者必须一定规模参与的承诺的一部分，这些对论坛的共享处于自愿（非承诺）。我们建议你对作者提问一些有挑战的问题以免他们失去兴趣！论坛和商品讨论的档案只要本书还在印刷将一直可以在出版社的网站访问。