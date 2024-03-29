1.I/O，可理解为In和Out
- I/O流：读写设备上的数据，硬盘文件、内存、键盘、网络……
- 根据数据的走向，可分为：输入流、输出流
- 根据处理的数据类型，可分为：字节流、字符流
- 字节流：可以处理所有类型的数据，如MP3、图片、文字、视频等。在读取时，读到一个字节就返回一个字节。在Java中对应的类都以"Stream"结尾。
- 字符流：仅能够处理纯文本数据，如txt文本等。在读取时，读到一个或者多个字节，先查找指定的编码表，然后将查到的字符返回。在Java中对应的类都以"Reader"或"Writer"结尾。

2.字符、字节与编码
- 字节(Byte)。是通过网络传输信息或在硬盘或内存中存储信息的单位，是计算机信息技术用于计量存储容量和传输容量的一种计量单位。1个字节等于8位二进制。
- 字符(Char)。是人们使用的记号，抽象意义上的符号。
- 字符集(Charset)。也称作“编码”。各个国家和地区所制定的不同ANSI编码标准中，都只规定了各自语言所需的“字符”。
- 字符集包含的含义：1、使用哪些字符。即哪些汉字，字母或符号会被收入标准中。所包含“字符”的集合就叫做“字符集”。2、规定每个“字符”分别用一个字节还是多个字节存储，用哪些字节来存储，这个规定就叫做“编码”。
- ANSI。不同ANSI编码所规定的标准是不相同的。
- UNICODE。对于UNICODE字符串来说，不管在什么环境下，它所代表的“字符”内容总是不变的。

3.读写数据
- BufferedReader及BufferedWriter带有缓冲区。即，可以将缓冲区写满后再对硬盘操作，减少了硬盘的使用次数。
- PrintWriter是打印的，可以用println()方法输出换行符。
- 缓冲写入数据的时候，如果缓冲没有写满，可能不会对硬盘进行写操作，此时关闭会导致数据丢失。需要先调用flush()方法进行写入。
- PrintWriter在创建的时候可以指定autoFlash，即对缓冲区的内容自动进行刷新写入。
