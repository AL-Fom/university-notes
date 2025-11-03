## Threat 1: Communication Interception
All types of media that uses nodes can be wiretapped (and sometimes eavesdropped)
Eavesdropping - monitoring traffic without extra effort
	usually done when the attacker is a legitimate user of a node through which packets pass through. Commonly known as packet sniffing
Wiretapping -
	passive - monitoring network traffic
	active - modifying messages

the vulnerability is due to HTTP being insecure (no encryption so everything is plaintext)
the security threats?
	confidentiality - subject to man in the middle and eavesdropping
	integrity - man in the middle alteration of messages

HTTPS is the secure version of HTTP which uses TLS (transport layer security) to encrypt all communication. 
HTTP
TLS (encapsulation down, decapsulation up)
TCP
IP

Some other threats to http:
	web logs - logging software at the server stores URL requests on disk (confidentiality) and users without permission can view sensitive data  (confidentiality)
	shoulder surfing - URL is displayed in the toolbar. sensitive data can be read, if they are in viewing range (confidentiality)
	browser cache - cache stores decrypted web pages (confidentiality)
	browser history - stores URL in full (confidentiality)

![[Pasted image 20251103093401.png]]

## Threat 2: Cookie theft
if you have cookie you dont need to crack username and password
to steal this you would have to access a badly developed website that use HTTP and HTTPS
	i.e. login via HTTPS but requests are HTTP 
	- packet sniffing on unsecure network will see the session in plain text

session hijacking - stealing valid session ID to get into the system and snoop the data
	predictable session ID
	session ID passed in URL
	Does not rotate session ID's
	Does not properly invalidate session IDs. (gives attacker longer time to get hold of it)

## Threat 3: Forced Browsing Attack
enumerating and accessing resourcing that are not referenced by application
an attacker can brute force to find unlinked content in the domain directory, such as temporary directories and files, and old backup and configs
this attack is performed manually when the app index directories are based on number gen or predictable values 

ensure role based authentication and auth for all resources to mitigate this.
hiding things doesnt mean its inaccessible and so  needs to be stored elsewhere.
avoid using common names for directories like admin, images, img
block access to unused file types so that only .html, .htm, .php and some other image extension are allowed



XSRF (CSRF) - CROSS-SITE REQUEST FORGERY
	bad website forces the user's browser to send a request to a good website
XSS (CSS) - CROSS-SITE SCRIPTING
	malicious code injected into trusted context (e.g. malicious data presented by a trusted website as code by user's browser)
SQL INJECTION 
	malicious data sent to a website interpreted as code in a query to the websites back-end