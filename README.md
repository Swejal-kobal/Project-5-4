# Project-5-4
Computer.hdl
ComputerRect.tst

CHIP Computer {

 IN reset;

  PARTS:
  	ROM32K(address=pc,out=instruction);
  	CPU(inM=inM,instruction=instruction,reset=reset,outM=outM,writeM=writeM,addressM=addressM,pc=pc);
  	Memory(in=outM,load=writeM,address=addressM,out=inM);
  }
![image](https://github.com/user-attachments/assets/d5fb0b31-0c53-40d4-a07c-fd378cbbf520)
