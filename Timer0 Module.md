- Readable and writable 8-bit timer/counter
- has an internal clocl cycle and external clock
- triggers interrupt during overflow
- OPTION_REG
	- Bit 5 TOCS
		- Clock source Select 
			- internal instruction cycle clock use its oscilator
	- BIT 4 TOSE
		- Source edge select bit
			- when will it trigger
				- high to low?
				- low to high
	- BIT 3 PSA
		- Prescaler clock divider
		- to reduce frequency
		- sets who to assign prescaler
			- 1 = Prescaler is assigned to the WDT
			- 0 = Prescaler is assigned to the Timer0 module
	- but 2-0 PS2:PS0 
		- Prescaler Rate Select Bits
		- 1:32 please use 100
- 11000100

- INTCON
	- GIE
	- TIMER0IE
		- enable 
	- TIMER0IF 
		- value if interrupt occurs
		- need manual reset after reading
	- 
```c
OPTION REG = 0xC4;
INTF = 0;
INTE = 1;

TMROIF = 0;
TMROIE = 1;

GIE = 1;
```