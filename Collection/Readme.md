# About Collection Framework in Java.  

## What Is a Collections Framework?
A collections framework is a unified architecture for representing and manipulating collections. --References from [Java official doc online](https://docs.oracle.com/javase/tutorial/collections/intro/index.html)  

集合框架是用于表示和操作集合的统一体系结构.  

 All collections frameworks contain the following:  
 所有的集合框架包含以下内容:  

 - Interfaces: These are abstract data types that represent collections. Interfaces allow collections to be manipulated independently of the details of their representation. In object-oriented languages, interfaces generally form a hierarchy.  
 接口：接口是表示集合的抽象数据类型。接口允许对集合进行独立于其表示细节的操作（即对操作抽象，不做细节实现）。在oo（面向对象）的语言里，接口通常构成一个层次结构。  

- Implementations: These are the concrete implementations of the collection interfaces. In essence, they are reusable data structures.  
实现：实现是接口的具体实现。本质上来讲，它们是可复用的数据结构。

- Algorithms: These are the methods that perform useful computations, such as searching and sorting, on objects that implement collection interfaces. The algorithms are said to be polymorphic: that is, the same method can be used on many different implementations of the appropriate collection interface. In essence, algorithms are reusable functionality.  
算法：算法是实现集合接口的执行有用的计算的方法，如搜索和排序。算法被认为是多态的，也就是说，同样的方法能够被不同的集合接口使用。本质上来说，算法是可复用的功能。  

集合框架中核心构成如下图所示  
![Collection，image froms Java official doc online](https://docs.oracle.com/javase/tutorial/figures/collections/colls-coreInterfaces.gif)  

###  Collection  
1.[Set](./Set)  
- SortedSet  

2.[List](./List) 

3.[Queue](./Queue)

4.Deque

###  Map  
1.[Map](./Map)  
- SortedMap