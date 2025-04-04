# invalid_command_program


## Description

This program simulates a dynamic array and processes a series of commands from an input file (`commands_2.txt`). The commands involve adding elements to the array (`PUSH`) and removing the last element (`POP`). Invalid commands, such as attempting to `POP` from an empty array or `PUSH` a negative value, are recorded in an output file (`invalid.txt`).

The program also handles edge cases such as missing values for `PUSH` commands and invalid command syntax.

## Features
- **Dynamic Array**: The program uses a dynamic array that automatically resizes when the number of items exceeds its current capacity.
- **Command Processing**: The program processes commands from an input file and handles errors by writing invalid commands to an output file.
- **PUSH Command**: Adds a positive integer value to the dynamic array. Negative values are considered invalid.
- **POP Command**: Removes the most recently added element from the array. If the array is empty, the command is invalid.
- **Invalid Command Logging**: Any invalid command (e.g., `PUSH` with a negative value, `POP` on an empty array, etc.) is logged into the `invalid.txt` output file.

## Input Format (`commands_2.txt`)
The input file contains a sequence of commands. Each command is represented by a command ID, followed by either the `PUSH` or `POP` command. If the command is `PUSH`, a positive integer value is provided. Here is an example of the input format:

Example input (invalid.txt):
INVALID COMMANDS
0
1
2
3
4
5
6
11
12
13
18
21
23
24
25
27
30
33
37
38
39
43
44
45
46
47
48
49
50
52
54
55
56
57
58
61
62
63
64

Example output (commands_2.txt):
0	POP	
1	PUSH	-40
2	PUSH	-21
3	PUSH	-30
4	POP	
5	POP	
6	POP	
7	PUSH	2
8	PUSH	13
9	POP	
10	PUSH	2
11	PUSH	-9
12	PUSH	-23
13	PUSH	-13
14	PUSH	11
15	PUSH	7
16	POP	
17	PUSH	6
18	PUSH	-38
19	PUSH	1
20	POP	
21	PUSH	-30
22	POP	
23	PUSH	-5
24	PUSH	-31
25	PUSH	-39
26	POP	
27	PUSH	-3
28	POP	
29	POP	
30	POP	
31	PUSH	10
32	POP	
33	PUSH	-18
34	PUSH	13
35	PUSH	9
36	PUSH	1
37	PUSH	-1
38	PUSH	-35
39	PUSH	-11
40	POP	
41	POP	
42	POP	
43	PUSH	-36
44	POP	
45	POP	
46	POP	
47	PUSH	-24
48	POP	
49	POP	
50	PUSH	-28
51	PUSH	12
52	PUSH	-4
53	POP	
54	POP	
55	PUSH	-25
56	POP	
57	POP	
58	PUSH	-9
59	PUSH	12
60	POP	
61	POP	
62	POP	
63	PUSH	-9
64	POP	
