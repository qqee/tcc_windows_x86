
# tcc_windows_x86

Tiny C language compiler

-------------------------------------------------------------

<h3>my patchs:</h3>

<h5>1. Support [naked] function. You can build clean opcode.</h5>
```c
__declspec(naked) void f(){
	asm("jmp 0x10001000");
	asm("ret");
}
```
<h5>2. Support [emit] to embed opcodes. 32bit [0x00~0xFF] continuous embedding.</h5>
```c
void f(){
	asm("_0x0");
	asm("_0xa;_0x0a;_0XA;_0X0A");
	asm("_0x00;_0x8;_0X0A;_0x0c;_0xF;_0XAA;_0xee");
}
```

-------------------------------------------------------------

Official website: <a target="_blank" href="http://www.tinycc.org">www.tinycc.org</a>

Finally released version [v0.9.26] is too old.

So I had to patch and compile it. Enjoy~ :notes:

-------------------------------------------------------------

qq@qq.ee





