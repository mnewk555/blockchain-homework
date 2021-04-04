# blockchain-homework

Matthew Newkirk UW FinTech Bootcamp Part-Time Apr. 2021 Unit 18 Homework - Blockchain

Network Name: mnewk_hw18
Chain id: 180

Network Start Procedure:
1. Open GitBash, navigate to network directory, execute the following command:
./geth --datadir node1 --unlock "b596c862FFD51548EE9c89b001133E62702b382c" --mine --minerthreads 1

2. Open another GitBash terminal, navigate to network directory, execute the following command:
./geth --datadir node2 --unlock "d5D670021B669CfA5ADf9E97a619e5dfa5ef18C2" --password "" --allow-insecure-unlock --mine --port 30304 --rpc --bootnodes "enode://c7c64440aba921cc09ce5bd4daa26be1d2042f5cbb260b07959725bf3c0028f96968068d1b2cf54a46cc2e17d016a0f1a6388a7a59b4877910795f088f5ff9f3@127.0.0.1:30303" --ipcdisable

Explanation of geth commands flags:

--datadir Points to the file folder of the node to be run.
--mine Activates minining.
--unlock Unlocks the account such that it can send transactions.
--minerthreads Number of CPU threads to use for mining.
--port Select port for node usage.
--bootnodes Points to the address of the first node for node linkage.
--rpc Enable remoted procedure calls so as to interact with node1.
--allow-insecure-unlock Bypass security for unlock with HTTP open.
--ipcdisable Disable the IPC-RPC server for the sake of Windows compatibility.
