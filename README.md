# NAND2Tetris Projects

These are the official project files for the NAND2Tetris Course.

For downloads of the Java simulator, [click here](https://www.nand2tetris.org/software).

For the web ide, [click here](https://nand2tetris.github.io/web-ide/).

## 门

引脚：单位引脚用单个小写拉丁字母表示，多位引脚用单个大写拉丁字母表示。

结果：0、1

优先级：()、'、与非 ,、& | \、> <、:

与非门（Nand）：ab

非门（Not）：a': a1

与门（And）：a&b: (ab)'

或门（Or）：a|b: a'b'

异或门（Xor）：a\b: (a&b')|(a'&b)

多路选择器（Mux）：a,b>s: (a&s')|(b&s)、a,b,c,d>s,t: (a,b>s),(c,d>s)>t

多路分配器（DMux）：a<s: (a&s'),(a&s)、a<s<t（四路）

多位门：AB、A'、A|B 等等

多路或门：a|b|c|d