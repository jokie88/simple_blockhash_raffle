# Simple Blockhash Raffle
A Simple Random Number Picker using a Future Blockhash on Bitcoin

This is a simple javascript page that generates a number between a specified range using the blockhash as the seed. Raffle organizer announces a future blockheight whose blockhash will be used to run a raffle. By entering the blockhash into this tool, you can determine the winning number within a range of values (e.g. 1-10,000). This can be mapped to an array of sorted inscription numbers to find the winning inscription/address etc. Its considered random 'enough' for a reasonble raffle. (see limitations below)

How it works:
- take the blockhash and convert it to a BigNum
- mod based on the range of values
- add offset to get adjust the range to be between min and max

  
Limitations:
- Is random to the extent that blockhashes are random
- Raffle is inconsequential enough that miners do not have an incentive to try to tip the scales by witholding blocks
- the range is small enough (lets say under several million items) that the 
- read more [here](https://ethereum.stackexchange.com/questions/94945/can-we-use-block-hash-as-verifiable-randomness-for-the-off-chain-lottery)


### [Simple Blockhash Raffle Tool](https://jokie88.github.io/simple_blockhash_raffle/blockhash_raffle.html)


[View Source on Github](https://github.com/jokie88/simple_blockhash_raffle/)
