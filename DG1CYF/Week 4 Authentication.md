Authentication is establishing identity of a user of an IT system
	user could be person or another IT system
	based on user knowledge shared by user and the system
The mechanisms can be any of the following:
	User knows
	User has
	What the user is
	Where the user is

Password threats
	Disclosure (Inadequate guarding)
	Inference (Pattern, predictable algorithm password)
	Exposure (Release of password)
	Loss (Forgetting)
	Snooping (Keyloggers, Network sniffing)
	Guessing (Limited choice, common passwords)
	Cracking (Automated "guessing")
	Multiple usage (Repeating on different platrforms)

Auth System:
	Auth info: user supplies to prove identity (username, password)
	Complementary info: stored on computer to validate auth info (set of encrypted password)
	Complementation function: what creates the complementary function (encryption function)
		for example: user password > same password in cleartext in db > identity function if password == password

Hashing:
- one way 
- same input will generate same hash
