### Proof of Work (High Cost in Compute and Energy)

The proof of work consensus protocol is best explained as a race.  Consensus is achieved by having all participating nodes solve a puzzle. The puzzle is a one-way translation of an amount of information consisting of the following items:

* All the data that present the transactions in the block - all the data is known by all participating nodes

* The number of the previous block.  Remember a blockchain links blocks of information together.

* A (variable) number.  This number is the part that can be changed.

The "work" is done by changing the variable number and see what the translation of all data brings.  The translation of all this data is a new number, and the requirement is that that number needs to be smaller than what is known as the “difficulty level”.  The difficulty level number has a fixed amount of numbers but when the first digits of the number are zero the overall number is lower.  So a higher difficulty is built by having a number that has more zeros at the start in the difficulty number.

Once the block is completed, all nodes will get the complete block of transactional data, everyone knows the previous block number and will start to change the variable number to get output from the puzzle algorithms comparing it to the required difficulty level.

The node that will find the number first will announce that is has found a solution matching the required difficulty level and the variable number of shared with all nodes in the network to verify that his solution is correct.  If a large portion of the nodes have verified the solution to be valid the solution is accepted and the block is added to the chain because consensus is reached.