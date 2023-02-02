# Binary Number System 

## Binary  Number System 

THe binary number system , also called the base-2 number system , is a method of representing numbers that counts by using combinations of only two numerals:
zero (0) and one(1). Computers use the binary number system to mainpulate and store all of their data including numbers, words ,vidoes, graphics and music 

The term bit, the smallest unit of digital technology, stands for "BInary digiT." A byte is a group of eight bits. A kilobyte is 1,024 bytes or 8,192 bits.

Using binary numbers, 1 + 1 = 10 because "2" does not exist in this system. A different number system, the commonly used decimal or base-10 number system, counts by using 10 digits (0,1,2,3,4,5,6,7,8,9) so 1 + 1 = 2 and 7 + 7 = 14. Another number system used by computer programmers is the hexadecimal system, base-16 , which uses 16 symbols (0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F), so 1 + 1 = 2 and 7 + 7 = E. Base-10 and base-16 number systems are more compact than the binary system. Programmers use the hexadecimal number system as a convenient, more compact way to represent binary numbers because it is very easy to convert from binary to hexadecimal and vice versa. It is more difficult to convert from binary to decimal and from decimal to binary.

The advantage of the binary system is its simplicity. A computing device can be created out of anything that has a series of switches, each of which can alternate between an "on" position and an "off" position. These switches can be electronic, biological, or mechanical, as long as they can be moved on command from one position to the other. Most computers have electronic switches.

When a switch is "on" it represents the value of one, and when the switch is "off" it represents the value of zero. Digital devices perform mathematical operations by turning binary switches on and off. The faster the computer can turn the switches on and off, the faster it can perform its calculations.

| Binary number System    | Decimal number system  | Hexadecimal number system   |
| :---        |    :----:   |          ---: |
| 0    | 0      | 0   |
| 1    | 1      | 1   |
| 10   | 2      | 2   |
| 11   | 3      | 3   |
| 100  | 4      | 4   |
| 101  | 5      | 5   |
| 110  | 6      | 6   |
| 111  | 7      | 7   |
| 1000 | 8      | 8   |
| 1001 | 9      | 9   |
| 1010 | 10     | A   |
| 1011 | 11     | B   |
| 1100 | 12     | C   |
| 1101 | 13     | D   |
| 1110 | 14     | E   |
| 1111 | 15     | F   |
| 10000| 16     | E   |



## Positional Notation
Each numeral in a binary number takes a value that depends on its position in the number. This is called positional notation. It is a concept that also applies to decimal numbers.

For example, the decimal number 123 represents the decimal value 100 + 20 + 3. The number one represents hundreds, the number two represents tens, and the number three represents units. A mathematical formula for generating the number 123 can be created by multiplying the number in the hundreds column (1) by 100, or 102; multiplying the number in the tens column (2) by 10, or 101; multiplying the number in the units column (3) by 1, or 100; and then adding the products together. The formula is: 1 × 102 + 2 × 101 + 3 × 100 = 123.

This shows that each value is multiplied by the base (10) raised to increasing powers. The value of the power starts at zero and is incremented by one at each new position in the formula.

This concept of positional notation also applies to binary numbers with the difference being that the base is 2. For example, to find the decimal value of the binary number 1101, the formula is 1 × 23 + 1 × 22 + 0 × 21 + 1 × 20 = 13.

## Binary Operations 
Binary numbers can be manipulated with the same familiar operations used to calculate decimal numbers, but using only zeros and ones. To add two numbers, there are only four rules to remember:

Therefore, to solve the following addition problem, start in the rightmost column and add 1 + 1 = 10; write down the 0 and carry the 1. Working with each column to the left, continue adding until the problem is solved.

To convert a binary number to a decimal number, each digit is multiplied by a power of two. The products are then added together. For example, to translate the binary number 11010 to decimal, the formula would be as follows:

To convert a binary number to a hexadecimal number, separate the binary number into groups of four starting from the right and then translate each group into its hexadecimal equivalent. Zeros may be added to the left of the binary number to complete a group of four. For example, to translate the number 11010 to hexadecimal, the formula would be as follows:

## Digital Data
Bits are a fundamental element of digital computing. The term "digitize" means to turn an analog signal—a range of voltages—into a digital signal, or a series of numbers representing voltages. A piece of music can be digitized by taking very frequent samples of it, called sampling, and translating it into discrete numbers, which are then translated into zeros and ones. If the samples are taken very frequently, the music sounds like a continuous tone when it is played back.

A black and white photograph can be digitized by laying a fine grid over the image and calculating the amount of gray at each intersection of the grid, called a pixel . For example, using an 8-bit code, the part of the image that is purely white can be digitized as 11111111. Likewise, the part that is purely black can be digitized as 00000000. Each of the 254 numbers that fall between those two extremes (numbers from 00000001 to 11111110) represents a shade of gray. When it is time to reconstruct the photograph using its collection of binary digits, the computer decodes the image, assigns the correct shade of gray to each pixel, and the picture appears. To improve resolution, a finer grid can be used so the image can be expanded to larger sizes without losing detail.

A color photograph is digitized in a similar fashion but requires many more bits to store the color of the pixel. For example, an 8-bit system uses eight bits to define which of 256 colors is represented by each pixel (28 equals 256). Likewise, a 16-bit system uses sixteen bits to define each of 65,536 colors (216 equals 65,536). Therefore, color images require much more storage space than those in black and white.



## Source 

- [encyclopedia.com](https://www.encyclopedia.com/computing/news-wires-white-papers-and-books/binary-number-system)
