### Proof of (Block) Stake (Low Cost in Compute and Energy)

With proof of stake consensus algorithms, the consensus algorithm does not solve puzzles in a race to be the first.  The first step is to identify and allow a certain number of nodes to be part of the blockchain.  This is called a permissioned blockchain because you need to have permission to partake.  This permission is given by distributing stakes.

Proof of stake consensus mechanism is solving a puzzle, but the puzzle contains only static elements - not variables - based on different characteristics:

* The block number

* The content (part) of blocks a long time ago (>2000 blocks)

* The transaction number (between the first and the last transaction) in the block of the stake transfer transaction all participating nodes needs to to

* The current timestamp

All these numbers are fixed but the time stamp and every node in the block stake blockchain will solve this puzzle every second until the output of this puzzle matches the required difficulty level.  

To make sure the one node that has solved the puzzle to match the difficulty level cannot introduce information in the block which allows him to tamper with the next blocks this node cannot use his used stake for a period amount of time for creating new blocks.

The fact that the puzzle-solving includes historic block data and once a node is assigned to create the block and put it on a chain will not be able to use that block state for a period of time makes it very costly to try to tamper with the content of the block (and the next blocks).