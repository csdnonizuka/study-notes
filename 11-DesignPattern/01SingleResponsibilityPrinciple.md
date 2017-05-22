### 单一职责原则的英文名称是Single Responsibility Principle， 简称是SRP。
SRP的原话解释是：
There should never be more than one reason for a class to change.
但是，基本上类的单一职责都用了类似的一句话来说"This is sometimes hard to
see"， 这句话翻译过来就是“这个有时候很难说”。
对于单一职责原则， 我的建议是接口一定要做到单一职责， 类的设计尽量做到只有一个
原因引起变化
### 里氏替换原则（ LiskovSubstitution Principle， LSP）
Java使用extends关键字来实现继承， 它采用了单一继承的规则， C++则采用了多重继承
的规则， 一个子类可以继承多个父类。 从整体上来看， 利大于弊
