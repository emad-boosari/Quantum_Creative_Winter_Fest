# Quantum_Creative_Winter_Fest

## Introduction
In this project, I am going to give a simple idea for shuffling cards for any game like *Poker*, *Black Jack* or high and low. In a card game, there is a preprocessing step for shuffling the cards which are normally performed by the dealer. I had always complained about the shuffling process and some dealers try to cheat during that. As you maybe know there is some technique for cheating in the card shuffling process. In the following project, I present a quantum circuit to generate a list of cards for playing. which is completely random and independent of the dealer's shuffling skill.

## Quantum Card Shuffling
Normally a deck of cards is 52 cards. Thus a system with 6 qubits can provide 64 basis states which is a little bit more than what we needed. For my purpose, I encoded the first 52 basis states as 52 playing cards and states from 53 to 64 here are meaningless. The following simple quantum circuit is a superposition of all basis states and after measurement gives us a 6-bit string of binary numbers corresponding to an integer. 
![image](https://user-images.githubusercontent.com/58440271/210639251-2ba781b9-2684-44ea-a8f2-ef20dba72889.png)

If the measured value is less than 53, then we can make a list in which the first card will be the outcome of the measurement. We must repeat the measuremnt until the length of the our list become 52. Then we are ready to play a Cards game!
