# NAND2Tetris Projects

These are the official project files for the NAND2Tetris Course.

For downloads of the Java simulator, [click here](https://www.nand2tetris.org/software).

For the web ide, [click here](https://nand2tetris.github.io/web-ide/).

## 门

引脚：单位引脚用单个小写拉丁字母表示，多位引脚用单个大写拉丁字母表示。要访问多位引脚的某一位，可用A.0

数值：0、1、#0101（二进制，以0开头）或#26（八进制），可以使用下划线分隔数字 #1001_0010

定义： = 

赋值：a<s:c,d

语句分隔符：;

优先级：()、#、'、.、与非 ,、& | \、> <、:、;、 = 

与非门（Nand）：ab

非门（Not）：a' = a1

与门（And）：a&b = (ab)'

或门（Or）：a|b = a'b'

多路或门：a|b|c|d|…

异或门（Xor）：a\b = (a&b')|(a'&b)

多路选择器（Mux）：a,b>s = (a&s')|(b&s)、a,b,c,d>s,t = (a,b>s),(c,d>s)>t

多路分配器（DMux）：a<s:i,j = a&s':i; a&s:j、a<s<t:c,d,e,f（四路） = a<s:i,j; i<t:c,d; j<t:e,f

多位门：AB、A'、A|B 等等

## ALU

半加器：a+b:c,s = a&b:c; a\b:s

全加器：a+b,c:r,s = a+b:i,t; t+c:j,s; i|j:r

加法器：A+B:c,S = A.0+B.0:r,S.0; A.1+B.1,r:i,S.1; …

自增器：A+1

算术逻辑单元：