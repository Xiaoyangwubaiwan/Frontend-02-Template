学习笔记

1. 本周学习总结
    
    对Number那一块，仿佛回到了大一学计算机基础的东西。
    String 转换Number  UIntArray 类型
    对象 
          1。Configurable 通过delete删除属性
        2。Enumerable 通过for-in循环返回属性
        3。Get 读取属性时调用的函数，默认值为undefined
        4。Set 写入属性时调用的函数，默认值为undefined
    new 方法实现
    思路：需要明白new到底做了什么
    生成一个新的实例对象
    实例对象__proto__链接到构造函数的prototype对象
    绑定构造函数的上下文为当前实例 获取参数，传入参数，并调用构造函数