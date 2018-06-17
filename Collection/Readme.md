# About Collection Framework in Java 8.  

## What Is a Collections Framework?
A collections framework is a unified architecture for representing and manipulating collections. --References from [Java official doc online](https://docs.oracle.com/javase/tutorial/collections/intro/index.html)  

集合框架是用于表示和操作集合的统一体系结构.  

 All collections frameworks contain the following:  
 所有的集合框架包含以下内容:
 - Interfaces: These are abstract data types that represent collections. Interfaces allow collections to be manipulated independently of the details of their representation. In object-oriented languages, interfaces generally form a hierarchy.  
 接口：接口是表示集合的抽象数据类型。接口允许对集合进行独立于其表示细节的操作（即对操作抽象，不做细节实现）。在oo（面向对象）的语言里，接口通常构成一个层次结构。
- Implementations: These are the concrete implementations of the collection interfaces. In essence, they are reusable data structures.  
实现：实现是接口的具体实现。本质上来讲，它们是可复用的数据结构。

- Algorithms: These are the methods that perform useful computations, such as searching and sorting, on objects that implement collection interfaces. The algorithms are said to be polymorphic: that is, the same method can be used on many different implementations of the appropriate collection interface. In essence, algorithms are reusable functionality.  
算法：算法是实现集合接口的执行有用的计算的方法，如搜索和排序。算法被认为是多态的，也就是说，同样的方法能够被不同的集合接口使用。本质上来说，算法是可复用的功能。