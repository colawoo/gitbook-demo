
### 1.ArrayList
- 基于数组实现，可以动态扩容。
- 线程不安全
- 有序
- 允许存储所有类型，包括null值
- 按索引查询，O(1)
- 没有排序的情况下，按照内容查询，O(n)
- 添加均摊，O(n)
- 插入和删除，O(n)

### 2.ArrayList扩容机制
在向ArrayList中添加元素的过程中，会判断当前底层的数组长度是否足够容纳所要存储的元素个数。如果不够，则会创建一个新数组，并将旧数组中的全部元素拷贝到新数组中。新数组的长度，一般来说是旧数组长度的1.5倍（oldCapacity + oldCapacity >> 1）。1 
