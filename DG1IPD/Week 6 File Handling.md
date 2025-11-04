Before reading a file must be opened
string = open("filename.txt", "permissions")
default permission is "r"
the file then needs to be closed at the end
name.close()

name.readline() will read only a single line

string[start:End] will create a substring between specified location
string.index() will find the position of a substring in a string
you can do something like 
	atSymbol = email.index()
	username = email.index([start:atSymbol])