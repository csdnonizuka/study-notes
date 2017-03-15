### Serializable和Parcelable两种序列化区别

1. 在使用内存的时候，Parcelable比Serializable性能高，所以推荐使用Parcelable。
2. Serializable在序列化的时候会产生大量的临时变量，从而引起频繁的GC。
3. Parcelable不能使用在要将数据存储在磁盘上的情况，
   因为Parcelable不能很好的保证数据的持续性在外界有变化的情况下。
   尽管Serializable效率低点， 也不提倡用，但在这种情况下，还是建议你用Serializable 。
### Android开发艺术探索P47
   Parcelable主要用在内存序列化上。
   Serializable用在将对象序列化到存储设备中或者将对象序列化后通过网络传输。
