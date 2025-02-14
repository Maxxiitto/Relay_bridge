![image](https://github.com/user-attachments/assets/065df45e-c604-479c-b3c9-899559fae21b)

Channel: https://t.me/shrimp_to_whale

**MAIN INFO**
- **Row-by-Row Data Processing**: Each line in `Evm_privates.txt` ALWAYS corresponds to the same line in `Eclipse_mnemonics_or_privates.txt` and `Proxies.txt` (e.g., line 1 in `Evm_privates.txt` matches line 1 in `Eclipse_mnemonics_or_privates.txt` and `Proxies.txt`, line 5 matches line 5, and so on).
- **Script supports bridging**
    - from almost any EVM chain
    - to almost any EVM chain + eclipse network
- **Results Logging**: Upon completion, all successful or failed accounts will be saved to Project_directory\Results\date-time folder in `Success.txt` and `Error.txt` files, respectively.


**Files that need to be filled out**

- `Eclipse_mnemonics_or_privates.txt` - private keys of your EVM accounts.
- `Eclipse_mnemonics_or_privates.txt` - private keys or mnemonics of your Eclipse accounts. (not mandatory)
- `Proxies.txt` - proxies in the api:port:login:password format.

**Settings**
 - Threads - number of threads
 - Retries - number of retries in case of failure
 - Delay - delay range (in seconds) between wallets
 - Shuffle wallets - (✓ - YES, □ - NO)
 - Bridge type:
    - range - bridge random number in specified range
    - max - bridge all ETH balance in specified network
 - Bridged from:
    - manual choise - fill out start network by yourself (Blast, Optimism, Zksync, etc.)
    - auto detection - soft will scan wallet balances in 3 popular networks (Arbitrum, Optimism, Base) and choose network with the highest ETH balance
 - Bridged to:
    - EVM chains - fill out destination network by yourself (Abstract, Scroll, Linea, etc.)
    - eclipse - bridge to eclipse network (`Eclipse_mnemonics_or_privates.txt` file must be filled out)
