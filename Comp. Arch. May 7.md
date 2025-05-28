### Detecting and Correcting Errors
[But what are Hamming codes? The origin of error correction](https://youtu.be/X8jsijhllIA?si=26pgCbtxZxC-HQb9) - 3Blue1Brown
[Hamming codes part 2: The one-line implementation](https://youtu.be/b3NxrZOu_CE?si=iC8J7R6ROxeKlTNO) - 3Blue1Brown
##### Error Detection
- Use a **parity bit** - a redundant bit used to check whether no bits are changed
	- detects even and odd single-bit errors
	- does *not* correct errors
	- even parity is 0 and odd parity is 1

- **Hamming distance** is the number of different symbols in a string
	- parity bits can only detect errors when the Hamming distance is 1
	- The scheme Hamming (7,4) is used to visualize the errors in the data or the parity bits

### Encoding
##### Fixed Length Encoding
- used for a finite set of variables like DNA or so
##### Variable Length Encoding
- one value can have multiple interpretations as shown below, when
	- a = 0
	- b = 1
	- c = 00
	- d = 11
- therefore:
		1) aaabbb = 000111 = 0-0-0-1-1-1
		2) acbd = 000111 = 0-00-1-11
		3) cabd = 000111 = 00-0-1-11
		4) acdb = 000111 = 0-00-11-1
		5) cadb = 000111 = 00-0-11-1
		6) aaabd = 000111 = 0-0-0-1-11
		7) aaadb = 000111 = 0-0-0-11-1
		8) acbbb = 000111 = 0-00-1-1-1
		9) cabbb = 000111 = 00-0-1-1-1
##### Huffman's Algorithm
 - solves the multiple interpretations downside that comes with variable length encoding
 - a minimum frequency algorithm that assigns prefix codes

	 j - 17 | o - 8 | h - 12 | a - 23 | n - 34
	
	o - 8 | h - 12 | j - 17 | a -23 | n - 34
	oh - 20 | j - 17 | a - 23 | n - 34
	joh - 37 | a - 23 | n - 34
	joh - 37 | an - 57
	johan - 94


### Logic Gates
 [CircuitVerse](https://learn.circuitverse.org)
 - NOT - one input, output returns flipped
 - AND - two inputs, if both are true, return true, otherwise false 
 - OR - two inputs, if any is true, then output true
 - NAND - opposite of AND gate, returns false if both inputs are true, otherwise return false
 - NOR - opposite of OR, returns true if both inputs are false, otherwise return false
 - XOR - two inputs, returns true if both inputs don't match
###### Truth table with 4 inputs (and 16 outputs)
	0 = 0000
	1 = 0001
	2 = 0010
	3 = 0011
	4 = 0100
	5 = 0101
	6 = 0110
	7 = 0111
	8 = 1000
	9 = 1001
	10 = 1010
	11 = 1011
	12 = 1100
	13 = 1101
	14 = 1110
	15 = 1111