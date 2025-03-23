What are the importance of crystal oscilators
- clock generation
- stable accurate timing
- instruction cycle determination 

The use of capicitors connected to crystal oscilators
- to stabilize and filter out noise


- pic16f877a
	- does not have an internal oscilator
	- which why we would require a crystal oscilator

A **current return path** is the path that electric current takes to return to the source after flowing through a circuit. **Electricity always flows in a complete loop**, meaning that for every current that leaves a voltage source (VCC), it must find a way to return.

- **In a DC circuit**, the current flows from the positive terminal of the power supply, through the circuit components, and back to the negative terminal (ground).
- **In an AC circuit**, the current alternates direction, but it still requires a defined return path to complete the loop.

- **For low-frequency DC circuits (e.g., PIC16F877A, LEDs, sensors)** → Use **ground as a return path**.
- **For high-speed signals (e.g., USB, Ethernet, RF, AC power systems)** → Use a **looped return path** for reduced noise.

A **pull-down resistor** is a resistor connected **between an input pin and ground (GND)** to ensure that the pin **reads a stable LOW (0V) state** when no other signal is present.

# Questions
- [ ] What are pull down resistors
	- [ ] what are pull down resistors and what are the purpose and how do we implement them?
what are floating
should we apply all floating to connect to ground?
would the other pins not connectedf to anything are called floating? and if so do we need to connect it to ground?
- [x] what is current return path and whats the difference of creating a loop rather to ground?