# Commands supported by my factorio computer
## 0. Group: Special
### blank instruction
**0**: -1

This is instruction does nothing

### set register to hardcoded value
**0**: -2
**A**: value
**B**: register number

This sets register (intended primary for jumps in code)

## 1. Group: Save
### constant to RAM (hardcoded)
**0**: 1
**A**: index
**B**: value

This saves constant to RAM (hardcoded)

### from register to RAM (hardcoded)
**0**: 2
**A**: index
**B**: pointer to value in registers

This saves value from target register to RAM (hardcoded)

### constant to RAM (address in registers)
**0**: 3
**A**: pointer to index in registers
**B**: value

This saves value from register in RAM (address in registers)

### from register to RAM (address in registers)
**0**: 4
**A**: pointer to index in registers
**B**: pointer to value in registers

This saves value from target register to RAM (address in registers)


## 2. Group: Load
### load from RAM (hardcoded)
**0**: 5
**A**: index
**B**: register number

This loads number from RAM (hardcoded) to given register

### load from RAM (address in registers)
**0**: 6
**A**: pointer to index
**B**: register number

This loads number from RAM (address in registers) to given register

## 3. Group: Basic arithmetic
### addition
**0**: 7
**A**: first operand
**B**: second operand
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### substraction
**0**: 8
**A**: first operand
**B**: second operand
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### multiplication
**0**: 9
**A**: first operand
**B**: second operand
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### division
**0**: 10
**A**: first operand
**B**: second operand
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### modulo
**0**: 11
**A**: first operand
**B**: second operand
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

## 4. Group: Basic comparison
### equal
**0**: 12
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### not equal
**0**: 13
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### greater than
**0**: 14
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### greater than or equal
**0**: 15
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### lower than
**0**: 16
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### lower than or equal
**0**: 17
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

## 5. Group: Basic boolean operation
### logical not
**0**: 18
**A**: first operand
**B**: unused
**C**: register that shall contain the result

This take a register A  and result will be saved in a register C.

### logical and
**0**: 19
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### logical nand
**0**: 20
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### logical or
**0**: 21
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### logical nor
**0**: 22
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### logical xor
**0**: 23
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### logical nxor
**0**: 24
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

## 6. Group bitwise operations
### bitwise and
**0**: 25
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### bitwise or
**0**: 26
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C

### bitwise xor
**0**: 27
**A**: first operand
**B**: second opernad
**C**: register that shall contain the result

This take a register A and a register B and result will be saved in a register C
