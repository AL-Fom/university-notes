Subject - entity that can perform tasks like a user or process
Object - entity on which operations happen
	Some can be both subject and object

Access Control Matrix - abstraction mechanism for specifying user operations on data
![[Pasted image 20251022094537.png]] 
Subjects S = { s1 ,…,s n }  
Objects O = { o1 ,…,o m }  
Rights R = { r1 ,…,r k }  
Entries A {s i, o j} ⊆ R  
A{s i, o j} = { r x, …, r y } means subject s i has rights r x, …, r y over object o j  
Typical rights: r(ead), w(rite), (e)x(ecute), a(ppend), o(wn)
	Can also be written as the following using Access Control Lists: 
		((s$_1$(r$_1$,$_1$ r$_1$,$_2$,...,r1$_1$,$_n$))(s$_2$(r$_2$,$_1$ r$_2$,$_2$,...,r1$_2$,$_n$)),..) This is useful for sparse access control matrices (matrix which is mostly empty)
			In a working example you would write: for f((bob, rwo), (alice, a)) or per subject ((f, rwo), (g, r), (p, rxwo), (q, w))

## Discretionary Access Control
a system that uses this allows owner of the resource to specify who can access which resources at the discretion of the owner
matrix with rows by IT sys subjects and columns by IT objects typically used by commercial orgs

## Role-based Access Control
![[Pasted image 20251022101153.png]]
This allows for fewer relationships to manage, orgs run based on roles which is more stable and easier to control than individually.

## Mandatory Access Control
decisions are made beyond the control of individual owner 
	central authority determines what info is accessed by whom
	user cant change rights
	typically is used by military


# Model Of Security
abstracts details of security policy (or set of) that are relevant for analysis 
	Policy to maintain confidentiality (Prevent unauthorized access to information)
		Bell-LaPadula model
		![[Pasted image 20251022112436.png]]
			each piece is ranked at a sensitivity level from unclassified to top secret following a "Need to Know" rule - access to sensitive data allowed only to subjects who need the data to perform their job and as such have clearance levels to not read anything that exceeds their level
			the main objective of this is to formally show computers can securely process classified information 
			formalization of military security defines the secure information flows because they describe acceptable connections between subjects and objects 
				Simple Security Property: subject may not read higher than current and lower sec level (No read-up)
				* (Star)-Property: subject may not write to lower than current and higher sec level (No write-down)  
	Policy to maintain integrity (Prevent unauthorized change to information)
		Biba model
			Simple Integrity Property: subject must not read lower level object (No read-down)
			Integrity * (Star)-Property: subject must not write to a higher level object (No write-up)

![[Pasted image 20251022114556.png]]