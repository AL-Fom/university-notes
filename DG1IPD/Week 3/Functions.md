Large chunks/blocks to make a program more manageable 
	A group of instructions performing some tasks
	can be invoked (called) as many times as needed in aa given program

Function structure:
	def name(v1, v2, v3):  <- function header with parameters/arguments
		----------  
		----------            <- function body or the block of code that you have decided to write in
		----------
	number of items in parameter list indicates how many values must be passed to the function
		after passing values into a function there are secnarios when you want thefunction to return i.e after a calculation

Mutable and Immutable parameters
	Depending on the language, how parameters are passed to a function determines whether changes are reflected in the back in the main program
	In Python
		Immutable
			Within functions: Numeric Types, Booleans, String, and Tuples are considered immutable 
				i.e if altered in function the value will NOT be reflected back in the main program
			unless explicitly returned using the return keyword
		Mutable
			In contrast, certain data types (passed as parameters), can be altered in the function without explicitly calling the return keyword these are considered mutable specifically when passing list and dictionaries 


Positional Parameters / Keyword Parameters
	a value assigned to a particular parameter based on position in parameter list 
		def mortgage_rate(amount, rate, term): 
				where mortgage_rate(350000, 0.06, 20)
			you can also use keywords within the parameters if you dont remember the function order
				mortgage_rate(350000, term = 20, rate = 6.5)
			You can also have default parameters so that if nothing is passe through it will default to given value
				mortgage_rate(amount, rate, term=20)



Variable Scope
	where a var is declared, influences its availability to the rest of your program code - this is var scope
		Variables declared outside of functions are global - they can be called throughout the program
		Variables declared inside of functions (not passed through as args) are local - they exist for the functions lifetime, and cease to exist after it terminates
	Local var example
		def func1():
			local_var = 5
		func1()
		print(local_var)
		will print nothing
	Global var example 
		global_var = 5
		def func1():
			print(global_var)
		func1():
		print(global_var)
		prints 5 for the function and 5 for the print statement


Comments 
	# is used as comment in python
	commenting is useful to know how a program works, they dont interact with the code
	You can also use docstring
	Represented with 3 ''' on each side of a comment
	