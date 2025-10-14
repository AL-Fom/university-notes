Vigenère cipher - Encryption alphabetic text using a series of interwoven shift ciphers, based on letters of a keyword

1. Choose a key e.g "Aston" (Numerical value of each letters is (0, 18, 19, 14, 13))
2. Split the text to be the same size as the key throughout 
3. Each letter give them their numerical value and another row below with the key values
4. Add the individual letters with the value from the key and mod 26 
![[Pasted image 20251013221019.png]]

To decrypt you would have to subtract the values from first row with values from 2nd row 