
### Computer Hardware
https://en.wikibooks.org/wiki/The_Computer_Revolution
- ###### Binary:
	 - refers to the base-2 number system, named for the only two digits, 0 and 1. We use the decimal number system, i.e. base-10 (named for the ten digits, 0 through 9).
	 - Computers use binary to store data, 0s and 1s, by using **bits**.
		 - eight bits become a **byte** which, using combinations of bits, can store up to 256 in binary
		 - 1024 bytes is a **kilobyte (KB)**. (1024 is 2^10, hence why that is used instead of a flat 1000)
		 - From here, it's more of the same. 1024 KB is equal to a **megabyte (MB)**, 1024 MB is a **gigabyte (GB)**, etc.
- ###### Motherboard
	- All parts of the computer connect to the motherboard. On its own, it's just a circuit board, but it's a necessary component, as it connects all other components.
- ###### Microprocessor
	- A microscopic processor, or **microprocessor** is simply miniaturized circuitry. It's in the name. CPUs are examples.
	- **Moore's Law** states that the number of transistors on a chip roughly double every two years, with minimal cost increase.
		- Importantly, this isn't set in stone, it's just an observation that has held true since Intel co-founder Gordon Moore articulated in 1965. It's not a law of physics, it's a law of economics.
		- As chips keep getting smaller, we may see Moore's Law fail sometime in the 2020s.
- ###### CPU
	- Central Processing Unit, the brain of the computer, and it handles most processes in a computer.
	- Multi-core CPUs speed up multi-tasking, and can handle separate tasks better than a single-core CPU can.
	- It's connected directly to the motherboard.
	- Intel and AMD manufacture most chips.
- ###### Servers
	- Technically, all a server is a computer that sends and receives data over a network.
	- Servers are what power the internet, the videos we watch, the text we read, are all hosted on servers.
- ###### Power Supply
	- A device that provides a computer with power.
	- An **Uninterruptible Power Supply** or **UPS**, is essentially the same thing, but contains a battery, which keeps supplying power in the event that the electricity is out.
- ###### Ports
	- An interface point on that allows external devices to be connected to the computer, such as display, additional storage, printers, etc.
### Microprocessor Basics
https://en.wikibooks.org/wiki/Microprocessor_Design
- ###### Basic Theory
	- Consider a city. This city has two ports, on for importing good and the other for exporting goods. There are many highways throughout the city on which trucks carry these goods to where they are needed.
	- This city is our microchip. The ports are Input and Outputs, and the rest of the analogy will be made clear.
- **Clocking Speed**
	- Consider the speed of the trucks. The faster they go, the more goods get delivered. In our chip, this is the clocking speed, and measured in GHz (gigahertz).
	- There's a limit to this, because as in real life, the faster the trucks go, the more we risk accidents, and losing cargo, or data.
- **CPU Fabrications**
	- If we made the roads safer, the turns wider, add rails, etc, we can reach higher max speeds safer.
	- More transistors means more space for data to pass through.
- **Pipelining**
	- If there's only one truck, then deliveries need to wait for the truck to finish it's current task and return to the ports each time. More trucks mean more simultaneous deliveries.
- **Multi-cores**
	- More lanes mean more capacity for more trucks.
- **32-bit and 64-bit**
	- A 2 ton truck can carry more load than a 1 ton truck can. Chips with 64-bit architecture can provide more memory space than 32-bits can.
- **Cache**
	- Picture a warehouse in the loading bay where the most popular goods are stored between deliveries, to be shipped when they will be needed.
https://virtualmuseum.intel.com
https://cpuvisualsimulator.github.io
http://www.visual6502.org