- Creation of the Control Unit


### Steps:
1. create a function titled CU
```c
int CU(void)
{

}
```
1. create local variable 
	1. Q: unknown reason why we need to generate these local variable
		- PC (Program Counter) → Points to the next instruction in Program Memory.
		- IR (Instruction Register) → Holds the current instruction being executed.
		- MAR (Memory Address Register) → Holds the address of memory being accessed.
		- I/O Registers (AR, BR, etc.) → Used for data transfer (like registers in a CPU).
		- Memory System → Contains both Program Memory (instructions) and Data Memory (variables).
2. Create memory system
	1. why is the memory system 8 -bits wide 
		1. each cell holds 1 byte of data
	2. why does it need to be 2n number of cells implemented on an array 
		1. address space is determined by the number of address bits
	3. why is the address is 11 bits and 
	4. why starting address of the program memory is 00016 and 
	5. data memory starts at 40016
	6. what are address bits?
		1. determines how many unique memory locations a system can address
			1. each memory location has a unique address
			2. With **11 address bits**, you can address **211=20482^{11} = 2048211=2048 memory locations** (from `000₁₆` to `7FF₁₆` in hexadecimal).

