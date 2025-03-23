```c
#include <xc.h>

// Configuration bits
#pragma config FOSC = XT   // Oscillator Selection bits (XT oscillator)
#pragma config WDTE = OFF  // Watchdog Timer Enable bit (WDT disabled)
#pragma config PWRTE = ON  // Power-up Timer Enable bit (PWRT enabled)
#pragma config BOREN = ON  // Brown-out Reset Enable bit (BOR enabled)
#pragma config LVP = OFF   // Low Voltage Programming Enable bit (disabled)
#pragma config CPD = OFF   // Data EEPROM Memory Code Protection bit (disabled)
#pragma config WRT = OFF   // Flash Program Memory Write Enable bits (Write protection off)
#pragma config CP = OFF    // Flash Program Memory Code Protection bit (disabled)
```