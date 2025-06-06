---
title: CS - HM - Decryption, Compression Exam Questions
category: A-Level
subject: Computer Science
topic: Exam Practice
date: 2025-03-18
tags: [A-Level, Exchanging-Data, CS, Computer-Science]
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}

# Question 1
ii) 
# Question 2
a) 00001110 00000001 00010001
b) a= 00001110 00000001 00010001
     v= 01000001 01000010 01000011
     XOR= 01001111 01000011 01010010
c) The encryption is symmetric as it uses the same key to encrypt and then decrypt the data
d) Asymmetric encryption is more suited to over-the-internet transactions as it uses two separate keys as there is a public key that is shared with others but cannot decrypt data and there is a private key which is only known by one person and *can* decrypt the data. This is better for over-the-internet transactions as the public key which could be intercepted by a malicious actor wouldn't be able to decrypt data but the private key is not sent oti and cannot be intercepted so malicious actors have no way of decrypting your data. Whereas, in symmetric encryption, the same key is used to encrypt and decrypt data and so it is possible for malicious actors to intercept your key and intercept your data
# Question 3
a:i) Requires less bandwidth for users to download it 
a:ii) Should use lossless as it doesn't remove any data which would make the text incomprehensible and lossless compression is reversible
b) PLAN:
	Knowledge: define RLE and dictionary encoding and how they work, explain compression
	Application: explain how RLE would apply to the text, explain how dictionary encoding would apply to the text
	Evaluation: Decide which one to recommend. Explain downside of RLE: not enough repeated characters or words to use over dictionary. Upside of Dictionary: many repeated words(Romeo, name, call)
	WRITTEN:

# Question 4
a) 'primary key' - cant do
b:i) 'hash' is a function that provides a map between an arbitrary length input and a usually fixed length 
b:ii) An advantage of storing the password as a hash is that if the database is breached, it cannot be read by a hacker and they would need to know the hashing function to compare it to the original password as hashing is one-way
e)
```
function checkAccess(givenPassword, passwordHash, locked)
	hashed = hash(givenPassword)
	if hashed == passwordHash and locked == 0:
		return True
	else: 
		return False
	endif
endfunction
```

# Question 5
PLAN: 
	Knowledge: define symmetric and asymmetric encryption
	Application: when would symmetric be used, when would asymmetric be used. how does it help modern society (banks, website databases, etc..)
	Evaluation: upside of symmetric over asymmetric (or vice versa) for a use-case

# Question 6
a) Compression is the act of modifying data to reduce file size
b) CCCMMMCCCC
c) 4C1O3L5C1M1O5C

# Question 7
i) Run Length Encoding
ii) Reduces amount of space needed for photographs on website/Allows for more photographs to be stored on website servers and it reduces the amount of bandwidth used by users to view the pages and could possibly reduce time needed for the webpage to load

# Question 8
 If the user chooses to watch the video with lossless compression, they will be able to watch it in a much higher quality but may run into issues with buffering depending on the internet speeds and they will use much more bandwidth due to the greater size of the video file. If the user watches a video with lossy compression, they will use less bandwidth than lossless and may have less buffering issues but the quality of the video will be worse as lossy compression permanently removes data whereas lossless preserves the original data
# Question 9
PLAN: 
	Knowledge: Define symmetric encryption(private key encryption) and asymmetric encryption as encryption methods. Define what hashing is (one way etc.)
	Application: For hashing, hash passwords and PINs to store them. When communicating files from robot to user and to other robots, use asymmetric or symmetric encryption to protect files; sensitive files should use asymmetric, less sensitive should use symmetric
	Evaluation: Asymmetric vs Symmetric: asymmetric protects against malicious actors trying to intercept sensitive data. Hashing prevents passwords and PINs being stored as plaintext and being vulnerable if a database was hacked.
# Related Notes
[[Computer Science MOC]]
[[CS - HM - Exam Practice]]
[[CS - HM - Exchanging Data]]
[[CS - HM - Compression, Encryption, Hashing]]