## About ArrayList
Resizable-array implementation of the List interface. Implements all optional list operations, and permits all elements, including null. In addition to implementing the List interface, this class provides methods to manipulate the size of the array that is used internally to store the list. (This class is roughly equivalent to Vector, except that it is unsynchronized.)  

ArrayList 是List接口的可变数组实现。实现了List的全部可选操作，包括允许为null的元素。除了实现List接口，本类还提供了方法操作内部用来存储用的数组的大小。（本类大致相当于Vector，除了本类不是同步的，即不是线程安全的）。  

The size, isEmpty, get, set, iterator, and listIterator operations run in constant time. The add operation runs in amortized constant time, that is, adding n elements requires O(n) time. All of the other operations run in linear time (roughly speaking). The constant factor is low compared to that for the LinkedList implementation.  

它的size, isEmpty, get, set, iterator和listIterator 操作是以常量的时间运行。add 操作是以平均的常量时间运行，也就是说，添加n个元素需要时间复杂度为O(n)的时间。其他的全部操作是以线性的时间（大概而言）运行。相对于LinkedList实现，ArrayList的常量因子是较低的。（常量因子，what？？？）  

Each ArrayList instance has a capacity. The capacity is the size of the array used to store the elements in the list. It is always at least as large as the list size. As elements are added to an ArrayList, its capacity grows automatically. The details of the growth policy are not specified beyond the fact that adding an element has constant amortized time cost.  

每一个ArrayList实例都有一个容量。该容量是list存储元素的数组大小。它总是至少和list的大小一样大。当元素添加到一个ArrayList，它的容量会自动增长。具体的扩容策略并不会特别超出添加一个元素所均摊的时间成本。  

An application can increase the capacity of an ArrayList instance before adding a large number of elements using the ensureCapacity operation. This may reduce the amount of incremental reallocation.  
在添加大量元素前，应用程序可以使用 ensureCapacity 操作来增加 ArrayList 实例的容量。这可能减少递增式再分配的数量。  

**Note that this implementation is not synchronized.** If multiple threads access an ArrayList instance concurrently, and at least one of the threads modifies the list structurally, it must be synchronized externally. (A structural modification is any operation that adds or deletes one or more elements, or explicitly resizes the backing array; merely setting the value of an element is not a structural modification.) This is typically accomplished by synchronizing on some object that naturally encapsulates the list. If no such object exists, the list should be "wrapped" using the Collections.synchronizedList method. This is best done at creation time, to prevent accidental unsynchronized access to the list:

   List list = Collections.synchronizedList(new ArrayList(...));  

**注意:此实现不是同步的** 如果多个线程并发访问一个ArrayList实例，同时至少其中一个的线程修改了list的结构，它则必须外部同步。（一个结构性修改是任何添加或删除一个或多个元素，或者是明确地重置了内部的数组大小；仅仅设置一个元素的值不是结构性的修改。）在一些自然封装list对象完成同步是典型的。如果没有这样对象存在，该list则应该通过Collections的synchronizedList方法包装。为了防止意外的不同步访问该list，最好是在创建的时候，使用:  
  List list = Collections.synchronizedList(new ArrayList(...));  