### 类型转换
#### 隐式类型转换
数组转换成指针
大多数情况下数组自动转换成指向数组首元素的指针。（decltype关键字参数、取地址符(&)、sizeof、typeid 都不会发生这种转换）
指针的转换
0 或 nullptr 都能转换成任意指针类型。指向非常量的指针能转换成 void*。指向所有对象的指针都能转换成 const void*。
转换成常量
指向非常量的指针转换成指向相应常量类型的指针
#### 显式类型转换
显示转换即使用强制类型转换。
强制类型转换非常危险，尽量避免使用。
castname 有四种：static_cast、dynamic_cast、const_cast、reinterpret_cast 。它指定了执行哪种转换。
static_cast
任何类型转换，只要不包含底层 const，都可以用 static_cast