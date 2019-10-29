# Huffman archiver

This project was created in September 2019 as a homework for C++ course in Computer Science Center

It is an archiver which opens file in binary format and compresses it with huffman algorithm 

## Usage

Program consumes one of two keys: -c or -d for compressing and decompressing and two names of files: uncompressed and compressed

```
huffman [-v] (-c|-d) input_file output_file
```
Also you can give -v flag as second argument in command line for showing codes for each symbol 

## Example 1:

```
.\huffman -c input.bin output.txt
```
As result you will see 3 numbers:
```
14672
634
567
```
Which are:
* size of uncompressed file
* size of compressed file
* size of auxiliary data

## Example 2:
```
.\huffman -v -c example.bin output_file.txt
```
You will see
```
16 
5 32
0 98
100 97
101 105
1100 120
1101 255
111 99
```
Where last 6 lines are huffman codes for symbols (bytes) with numbers 97, 98, 99, 105, 120, 255
