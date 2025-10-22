Cryptanalysis is the study of and application of methods for extracting the meaning of encrypted information without access to the decryption key
For example exhaustive search:
	if the space is small enough you can try all possible combinations until you find the right one like in the shift cipher as there is only 25 possible keys

Different types of attack:
	ciphertext only -  the goal is to find plaintext, possibly the key from the ciphertext
	known plaintext - adversary has ciphertext and corresponding plaintext, goal is to find the key 
	chosen plaintext - adversary may supply plaintexts and obtain corresponding ciphertext, goal is to find the key

A way to perform a known plaintext on Vigenère is to search through all possible ciphertext until a repeating key is found 
![[Pasted image 20251014010311.png]]

# Transposition Ciphers
Transposition Cipher (Permutation Cipher) -  method of encryption which scrambles the position of characters
	Does not substitute one symbol for another, instead it changes the location of the symbols
Keyless transposition ciphers permute the characters by using writing plaintext and reading it another way 
	Rail Fence
Keyed transposition ciphers divide the plaintext into groups of predetermined size, called blocks and then use the key to permute the characters in each block separately
	Columnar 


Rail Fence Encrypting
Take phrase, write the plain text on n rows going down across up across down, read the rows such that it looks like this

HLORL          ->     HLORLEWOD
ELWOD


Rail Fence Decrypting
Take the phrase, write it out over given number of rows, read it as you wrote the text above so that it looks like this 

akan
tctw    ->      Attack At Dawn
tada   




Columnar Transposition 
![[Pasted image 20251014004034.png]]
