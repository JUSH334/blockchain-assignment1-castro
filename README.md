# blockchain-assignment1-castro
CS 476 - Assignment 1


HOW TO RUN
-------------------------------------------------------------------------------------

INSTALLATION AND SETUP
	
	1. Verify Node.js Installation:
		node -v
		npm -v
	2. Create Workspace
		mkdir -p ~/blockchain-activity && cd ~/blockchain-activity
	
HOW TO RUN

	1. Navigate to Project Directory
		cd ~/blockchain-activity-castro
		
	2. Execute the blockchain program
		node blockchain.js

EXPECTED OUTPUT

	Mining block #1 ...
	 Block mined (idx=1): 000a1b2c3d4e5f...
	 Mining block #2 ...
	 Block mined (idx=2): 000f5e4d3c2b1a...
	 Mining block #3 ...
	 Block mined (idx=3): 0009876543210a...
	
	 Full chain:
	{
	  "chain": [
	    {
	      "index": 0,
	      "timestamp": "...",
	      "data": "Genesis Block",
	      ...
	    },
	    ...
	  ],
	  "difficulty": 3
	}
	
	 Is chain valid? true
	
	 Tampering with block #1 data ...
	 Is chain valid after tamper? false

-------------------------------------------------------------------------------------

REFLECTION
-------------------------------------------------------------------------------------

This blockchain implementation provided valuable insights into the fundamental mechanics of cryptocurrency and distributed ledger technology. Working with cryptographic hashing demonstrated how SHA-256 creates a unique digital fingerprint for each block, where any modification to the data results in a completely different hash value. 

The Proof-of-Work mining process illustrated why blockchain networks require significant computational resources. The system must iterate through countless nonce values until it discovers a hash meeting the difficulty requirements. The chain validation mechanism was interesting when we tested tampering with transaction data. The blockchain detected the inconsistency because the recalculated hash no longer matched the stored value, effectively breaking the cryptographic chain. 

This assignment helped clarify why blockchain technology is considered tamper-resistant and how it enables trustless transactions between parties without requiring a centralized authority or a "third-party". Overall, building this blockchain from scratch helped me understand how these interconnected components work together to maintain data integrity and security in decentralized systems.

-------------------------------------------------------------------------------------

SCREENSHOTS
-------------------------------------------------------------------------------------

<img width="1906" height="1020" alt="Screenshot from 2025-09-01 16-12-11" src="https://github.com/user-attachments/assets/d153eb04-d9a4-4059-855d-f3f01a6751f9" />
<img width="1906" height="1020" alt="Screenshot from 2025-09-01 16-12-35" src="https://github.com/user-attachments/assets/5daeb738-f78f-45aa-99a1-9f240773ddbe" />


