# Assembler
This program was made by our group of three, as a part of our project for the CSE3015 Digital Logic Design course. It takes a set of instructions of the ISA we've specified and converts it to the machine code. After that, we send the machine code as input to the processor we've designed in Logisim.

For the program to work:
* Instructions must be written into the input.txt file that is within the same directory as the program.
* Instructions must be written as one per line.
* There must be a space between the parts of the instruction.

##  Instructions of the ISA
  <table>
    <tr>
      <th>Instruction</th>
      <th>[15:12] (Opcode)</th>
      <th>[11:9]</th>
      <th>[8:6]</th>
      <th>[5:3]</th>
      <th>[2:0]</th>
    </tr>
    <tr>
      <td>AND</td>
      <td>0001</td>
      <td>DR</td>
      <td>SR1</td>
      <td>SR2</td>
      <td>000</td>
    </tr>
    <tr>
      <td>ANDI</td>
      <td>0010</td>
      <td>DR</td>
      <td>SR1</td>
      <td colspan="2">IMM</td>
    </tr>
    <tr>
      <td>ADD</td>
      <td>0011</td>
      <td>DR</td>
      <td>SR1</td>
      <td>SR2</td>
      <td>000</td>
    </tr>
    <tr>
      <td>ADDI</td>
      <td>0100</td>
      <td>DR</td>
      <td>SR1</td>
      <td colspan="2">IMM</td>
    </tr>
    <tr>
      <td>LD</td>
      <td>0101</td>
      <td>DR</td>
      <td colspan="3">ADDR</td>
    </tr>
    <tr>
      <td>ST</td>
      <td>0110</td>
      <td>SR</td>
      <td colspan="3">ADDR</td>
    </tr>
    <tr>
      <td>CMP</td>
      <td>0111</td>
      <td>OP1</td>
      <td>OP2</td>
      <td colspan="2">000000</td>
    </tr>
    <tr>
      <td>JUMP</td>
      <td>1000</td>
      <td colspan="4">ADDR</td>
    </tr>
    <tr>
      <td>JE</td>
      <td>1001</td>
      <td colspan="4">ADDR</td>
    </tr>
    <tr>
      <td>JA</td>
      <td>1010</td>
      <td colspan="4">ADDR</td>
    </tr>
    <tr>
      <td>JAE</td>
      <td>1011</td>
      <td colspan="4">ADDR</td>
    </tr>
    <tr>
      <td>JB</td>
      <td>1100</td>
      <td colspan="4">ADDR</td>
    </tr>
    <tr>
      <td>JBE</td>
      <td>1101</td>
      <td colspan="4">ADDR</td>
    </tr>
  </table>
