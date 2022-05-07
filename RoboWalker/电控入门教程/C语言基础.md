# C语言基础

### 知识架构

##### 1. 基础

1. 看**规范文档**，掌握各种**语句**和**数据类型**。
2. 了解各种**运算符**。
3. 学习**顺序、选择、循环** 3种基本程序结构，掌握**if-else、for、while、do-while、switch-case、break、continue**等语句的用法，goto有所了解即可。

##### 2. 函数

1. **函数+参数类型+返回值**。
2. **局部与全局变量+变量存储类型+递归函数+内外部函数**。
3. 熟练使用函数简化程序，降低模块耦合度。

##### 3. 数组

1. 学习**遍历数组**并实现简单应用。
2. **字符串**与数组处理。

##### 4. 结构体

1. 学习结构体描述一个**对象**的思想

##### 5. 指针

1. 指针用于字符串操作

 	2. 指针用于**参数传递**

##### 6. **数据结构与算法**

1. 链表

 	2. 队列
 	3. 栈

---

### 需要强调的问题

#### STM32上数据的位数

在 "stdint.h" 中重命名了这几个类型

```c
    /* exact-width signed integer types */
typedef   signed          char int8_t;
typedef   signed short     int int16_t;
typedef   signed           int int32_t;
typedef   signed       __INT64 int64_t;

    /* exact-width unsigned integer types */
typedef unsigned          char uint8_t;
typedef unsigned short     int uint16_t;
typedef unsigned           int uint32_t;
typedef unsigned       __INT64 uint64_t;
```

#### 位运算的用法

```
&、|、^、~、>>、<<
```

```c
uint8_t num=0xAB,result;

result = num & 0xF0;
result = num >> 4;
num |= (0x01<<3);
num &= ~(0x01<<5);
```

#### 头文件的作用

模块化

#### 变量的生命周期和作用域

全局变量、静态局部变量、动态局部变量

#### 指针的作用

与传值相比，指针可以实现快速的信息传递

