Cryptanalysis is the study of and application of methods for extracting the meaning of encrypted information without access to the decryption key
For example exhaustive search:
	if the space is small enough you can try all possible combinations until you find the right one like in the shift cipher as there is only 25 possible keys

Different types of attack:
	ciphertext only -  the goal is to find plaintext, possibly the key from the ciphertext
	known plaintext - adversary has ciphertext and corresponding plaintext, goal is to find the key 
	chosen plaintext - adversary may supply plaintexts and obtain corresponding ciphertext, goal is to find the key

A way to perform a known plaintext on Vigenère is to search through all possible ciphertext words until a repeating key is found 
![[Pasted image 20251014010311.png]]