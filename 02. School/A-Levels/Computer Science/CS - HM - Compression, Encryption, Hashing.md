---
title: CS - HM - Compression, Encryption, Hashing
category: A-Level
subject: Computer Science
topic: Exchanging Data
date: 2025-03-18
tags: [A-Level, Computer-Science, CS, Exchanging-Data]
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}
# Compression
- There are two different types of compression:
	- **Lossy**: *Non-essential data is permanently removed*, e.g. different shades of the same colour in an image. - **non-reversible**
	- **Lossless**: *Using patterns to reduce the file size* - **reversible**
## Run Length Encoding (RLE)
- A basic method of *lossless* compression that summarises consecutive patterns of the same data.
- Doesn't work on images on where there is a lot of different patterns
- Works well with image and sound data where data could be repeated many times ![[Pasted image 20250318094338.png]]
## Dictionary Compression
- Spots regularly occurring data and stores it separately in a dictionary
- The reference to the entry in the dictionary is stored in the main file thereby reducing the original data stored
- Even though, the dictionary produces additional overheads, the space saving negates the problem
### Example
- Compress the phrase "no pain no gain" [15 bytes]
- This dictionary turns the phrase into 0001 1000 1110 [12 bits]

| Number | Entry | Binary |
| ------ | ----- | ------ |
| 1      | no_   | 00     |
| 2      | p     | 01     |
| 3      | ain_  | 10     |
| 4      | g     | 11     |

# Encryption
- A way of making sure data cannot be understood if you don't possess the means to decrypt it
- Two methods at the opposite end of the security spectrum are the Caesar Cipher and the Vernam Cipher - Low Security -> High Security
## Caesar Cipher
- The most basic type of **encryption** and the *most insecure*
- Letters of the alphabet are shifted by a consistent amount ![[Pasted image 20250318103937.png]]
## Brute Force Attack
- A **brute force attack** attempts to apply every possible key to decrypt ciphertext until one works
- Spaces are often removed to mask word lengths

## Vernam Cipher
- The *encryption key*, the one-time pad, is the only cipher proven to be unbreakable
- The key must be:
	- A truly random sequence greater or equal in length than the plaintext and only ever used once
	- Shared with the recipient by hand, independently of the message and destroyed immediately after use
## Decoding
- Encryption and Decryption of the message is performed bit by bit using an XOR operation with the shared key
## Symmetric Encryption
- Known as **Private Key Encryption**
- The same key is used to encrypt and decrypt data
- This means that the key must also be transferred to the recipient
- The key can be intercepted as easily as the ciphertext message which causes an obvious security problem so **Asymmetric Encryption** may be used
## Asymmetric Encryption
- Uses two separate but related keys
- One key, the public key, is made public so that others who want to send you data can use this key to encrypt it
	- The public key cannot decrypt the data
	- A private key, only known to you, is used to decrypt the data
# Hashing
- A hashing function provides a mapping between an arbitrary length input and a usually fixed length or smaller output 
- It is one-way - can *not* get back to the original
- Is useful for storing encrypted PINs and passwords so that they cannot be read by a hacker
	- To verify a user's password, the software applies the hash function to the user input and compares the hashed result with the one stored 
# Related Notes
[[Computer Science MOC]]