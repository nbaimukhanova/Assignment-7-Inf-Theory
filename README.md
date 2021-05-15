# Assignment-7-Inf-Theory

Goal: Add errors to the binary sequence after Part4 (Hamming code). Decode Hamming code and  fix errors. 

1. Read the file with the sequence of bits from assignment 7 and divide into blocks of  8 or 16 bits based on your Hamming code method from the previous assignment. Each member  of a team should have one method.

2. You will simulate the channel by randomly flipping each bit in each codeword with  a probability 30 – 50%. You will need to generate one error in one data bit of 30 – 50% blocks  randomly. For example, if you have 10 blocks, you will need to flip one data bit in 3-5 blocks. The  data bit you flip and the block you choose should be random. 
Write a function called ErrorGen(percent, bitstring), which takes as input a bitstring block to send  over a binary symmetric channel, and simulates flipping bits at a rate percent. It then returns the  corrupted string. 
 
3. You will also need a function HammingDecode(bitstring) that takes 8 or 16 bit  number (the output of the channel) and returns a guess at the 4 or 11 bit number originally sent. Include all intermediate steps. 

4. Run functions HammingDecode and HammingDecode2 on all data blocks. Please  include all intermediate steps. The output should be the same as in the previous output (3), but  on all data blocks. 

5. Combine all of the decoded bitstrings into one sequence. Print it and save it in a txt  file. Compare it with the with the sequence of bits from assignment 3. 
