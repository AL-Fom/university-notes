Secret writing concealing meaning 
	Strongest control against security threats 
Code - word or phrase that has meaning to those who know != Cryptography

Encryption (Encoding, enciphering) - the process of scrambling a message so that its meaning isn't obvious
Decryption (Decoding, deciphering) - Reverse 

Plaintext - Original message
Ciphertext - The encrypted message
Key - device used to influence the way in which encryption and decryption are carried out
Cryptosystem (Cipher) - System for encryption and decryption


Substitution cipher - replace every letter in the message with letter that is a fixed number of positions further along in the alphabet such that if you had ABC and shifted it by 5 it would become FGH
![[Pasted image 20251013215820.png]]

Modular arithmetic - When answer to a calculation must be in range 0 to m-1, where m is modulus
	ex. Result = 33 mod 26
	Result = 7 (Counting from 0 after 25) 


# Vigenère Cipher
Vigenère cipher - Encryption alphabetic text using a series of interwoven shift ciphers, based on letters of a keyword

1. Choose a key e.g "Aston" (Numerical value of each letters is (0, 18, 19, 14, 13))
2. Split the text to be the same size as the key throughout 
3. Each letter give them their numerical value and another row below with the key values
4. Add the individual letters with the value from the key and mod 26 
![[Pasted image 20251013221019.png]]

To decrypt you would have to subtract the values from first row with values from 2nd row 