favorite_code
=============

代码收藏

double.c中值得学习的地方：
  getword中的计算行数linenum的for循环
  getword中copy the word into buf[0..size-1]这里的for循环，一直getc直到空格，但只保存了前面size-1个字符
  getword中ungetc部分，可以保持程序健壮性，比如正好单词长度是size，这样就会少计算linenum
  double判断也很巧，先初始化赋值prev[0] = '\0'
