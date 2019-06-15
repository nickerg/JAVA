1.文件
- 文件的创建是基于当前工程文件夹的。
- 使用的是相对路径。
- file移动文件可以跨目录。但是必须在同一个分区。
- 可以通过rename进行重命名。不需要一个具体存在的文件
- 文件处于不同的分区，需要使用文件的拷贝。

2.文件夹
- mkdir()相当于mkdir；mkdirs()相当于mkdir -p。
- 文件夹可以单独一级重命名。
- 如果目标的文件/文件夹已经存在，则重命名会失败。

3.文件属性的读取
- exists()，判断文件是否存在
- getName()，读取文件名称
- getPath()，读取文件相对路径
- getAbsolutePath()，读取文件的绝对路径
- getParent()，获取文件的父级路径。 new File(file.getAbsolutePath()).getParent()。
- length()，读取文件大小，为字节byte。
- isHidden()，判断文件是否被隐藏。
- canRead()，判断文件是否可读。
- canWrite()，判断文件是否可写。
- isDirectory()，判断文件是否为文件夹。

4.文件属性的设置
- setWritable(true/false)。将文件设为可写？
- setReadable(true/false)。将文件设为可读？
- setReadOnly()。将文件设为只读。

5.文件的简单读写
- 写创建文件
- 根据文件创建文件输入流。FileInputStream
- 创建输入流读取。InputStreamReader
- 创建读取缓冲。BufferedReader
- 先创建的后关闭
- 需要对异常进行处理
