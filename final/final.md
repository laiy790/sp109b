# 期末專案 
## 程式的修改來源

+ 參考陳鍾誠老師的專案(C1-c4)

## 編譯器
+ 是一種電腦程式，它會將某種程式語言寫成的原始碼（原始語言）轉換成另一種程式語言（目標語言）。

+ 它主要的目的是將便於人編寫、閱讀、維護的進階電腦語言所寫作的原始碼程式，翻譯為電腦能解讀、執行的低階機器語言的程式，也就是執行檔。編譯器將原始程式（source program）作為輸入，翻譯產生使用目標語言（target language）的等價程式。原始碼一般為高階語言（High-level language），如Pascal、C、C++、C# 、Java等，而目標語言則是組合語言或目標機器的目的碼（Object code），有時也稱作機器碼（Machine code）。

### 編譯器工作流程
+ 原始碼（source code）→ 預處理器（preprocessor）→ 編譯器（compiler）→ 組譯程式（assembler）→ 目的碼（object code）→ 連結器（linker）→ 執行檔（executables）
## 簡介 -- C4 編譯器
+ [C4](https://github.com/rswier/c4) 是 [Robert Swierczek](https://github.com/rswier/) 寫的一個小型 C 語言編譯器
+ 原始碼都在 [c4.c](https://github.com/)
+ C4 編譯器的用法
    ```
    gcc -m32 -o c4 c4.c  (you may need the -m32 option on 64bit machines)
    ./c4 test/hello.c
    ./c4 -s test/hello.c

    ./c4 c4.c test/hello.c
    ./c4 c4.c c4.c test/hello.c
    ```
