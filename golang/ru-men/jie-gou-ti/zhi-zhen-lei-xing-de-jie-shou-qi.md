# 指针类型的接收器

指针类型的接收器由一个结构体的指针组成，更接近于面向对象中的this或者self

由于指针的特性，调用方法时，修改接收器指针的任意成员变量，在方法结束后，修改都是有效的。

这其实和JavaScript的深浅拷贝基本相同，关于指针和非指针的表现和作用就不再赘述了

#### 使用场景

在计算机中，小对象由于值复制时的速度较快，所以适合使用非指针接收器。

大对象因为复制性能较低，适合使用指针接收器，在接收器和参数间传递时不进行复制，只是传递指针。


