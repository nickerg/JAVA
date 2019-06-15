1.实例化String对象。
- 直接赋值
- 使用关键字 `new`
- 字符串比较多用"equals"，比较的是内容。
- 字符串内容不可更改。改变的是堆内存地址的指向。

2.String字符串常用方法。
- 字符串长度：length方法。
- 字符串转换数组：toCharArray()。
- 从字符串中取出指定位置的字符：charAt()。
- 与byte数组的转换：getBytes()。
- 过滤字符串中存在的字符：indexOf()。
- 去掉字符串的前后空格：trim()。
- 从字符串中取出子字符串：subString()。
- 大小写转换：toLowerCase() toUpperCase()。
- 判断字符串的开关结尾字符：endsWith() startWith()。
- 替换String字符串中的一个字符：replace()。

3.认识SringBuffer：
- 缓冲区，本身也是操作字符串，但是StringBuffer可更改。
- StringBuffer是一个操作类，所以必须通过实例化操作。
- StringBuffer常用方法：append() insert() replace() indexOf()。
- replace()是将原有范围的删除，然后插入替换的内容。

4.StringBuilder：
- 一个可变的字符序列，被设计作用StringBuffer的一个简易替换，用在字符串缓冲区被单个线程使用的时候。速度比StringBuffer快。
- 如果涉及到线程安全方面，建议使用StringBuffer。
