exception handling involves catching thrown errors by adding lines to work around them

in an embedded function it will call all the functions that call it to have an error

try:
	function
except ErrorType:
	function


you can raise errors i.e
if != result:
	raise Error("message)

as err: orirgnal exception to the print
OSError: no file found
Runtime: generic catch for all exceptions

finally block is must execute code so even without an error it will run