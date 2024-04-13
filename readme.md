# PBR Programming Language
## A basical interpreted turing language made in Python
Doc of FigJam :
![PBR Image Doc](assets/imgdocs.png)
(In FRENCH)

## Documentation  (English) :
The PBR was made for be very minimal (only 14 instructions). It's a stack based langage who works with piles (only 3 piles). The syntax are simple but programs are headache. It's a fast interpreted language made in Python.

### Syntax
One line, one instruction. You can write instructions in uppercase like in microcomputers or just in lowercase.

### Comments
This time, comments are very important in this language, it's the only way to navigate it. Some comments examples :
```asm
; I'm a comment (one-line only supported)
INSTRUCTION ; I'm a comment after an instruction
```

### Values
There is only one value type : integers. If you put a char at the place of a integer value, it will be converted in integer with it ASCII code.

### Piles available
There are 3 piles : the pile A and B for operations and the pile C for operations results or values isolation.

### Piles manipulation
`PUSH <pile> <value (only one)>` to append a value on the pile selected.
`POP <pile>` to pop a value on the pile selected, just remove the last value nothing else.
`MOVE <pile 1> <pile 2>` to move the last value of the pile 1 to the pile 2.
`COPY <pile 1> <pile 2>` to copy the last value of the pile 1 to the pile 2.

### Calculations with piles
`ADD` to additionate the last value of the pile A and the pile B and append the result to the pile C, the two elements from the calcul will be removed to their piles.
Same for `SUB` to substract, `MUL` for multiply and `DIV` for divide.

### Console interactions
`PRINT <pile>` to print the last value of the selected pile.
`INPUT <pile>
