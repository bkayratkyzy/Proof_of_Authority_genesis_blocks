# Proof of Authority Development Chain


In order to set up a testnet, you will need to use the following skills

* Puppeth, to generate your genesis block.

![puppeth](screenshots/puppeth.png)

* The Clique Proof of Authority algorithm.

![proof_of_authority](screenshots/proof_of_authority.png)


* Geth, a command-line tool, to create keys, initialize nodes, and connect the nodes together.


![creating_nodes](screenshots/creating_nodes.png)

* Connect nodes, make sure to unlock them 
* Run this command lines to unlock and mine 

../geth --datadir node1 --mine --rpc --unlock "0x784DbeBf24c882d912B28dc7A2dB2C61f8802828" --allow-insecure-unlock



*  Look for enode, you will need it to run next command , remember to change port number from 30303 to 30304

![enode](screenshots/enode.png)


../geth --datadir node2 --mine --unlock "0x10e53987124441E80013a0147E079B33B8B81d0E" --allow-insecure-unlock --bootnodes enode://a2693b5617cdf550f6e18057a4d39b4212c90669d5f48bd0fa1e25a7935460353028e7535203e86c6640003762216f89fd4278923d213ec20ea87ad6bcf1f3b9@127.0.0.1:30303 --port 30304


* Nodes are mining!

![node1_mine](screenshots/node1_mine.png)


![node2_mine](screenshots/node2_mine.png)

* Sending transactions on MyCrypto. Create custom network, make sure to use same chain ID. In order to have ETH in your account pre fund them when creating genesis block.

![transaction](screenshots/transaction.png)



