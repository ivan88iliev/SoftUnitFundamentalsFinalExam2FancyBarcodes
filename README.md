# SoftUnitFundamentalsFinalExam2FancyBarcodes
Problem 2. Fancy Barcodes

Your first task is to determine if the given sequence of characters is a valid barcode or not. 
Each line must not contain anything else but a valid barcode. A barcode is valid when:
•	Is surrounded with a "@" followed by one or more "#" 
•	Is at least 6  characters long (without the surrounding "@" or "#")
•	Starts with a capital letter
•	Contains only letters (lower and upper case) and digits
•	Ends with a capital letter
Examples of valid barcodes: @#FreshFisH@#, @###Brea0D@###, @##Che46sE@##, @##Che46sE@###
Examples of invalid barcodes: ##InvaliDiteM##, @InvalidIteM@, @#Invalid_IteM@#
Next you have to determine the product group of the item from the barcode. The product group is obtained by concatenating all the digits found in the barcode. If there are no digits present in the barcode, the default product group is "00".
Examples:  
@#FreshFisH@# -> product group: 00
@###Brea0D@### -> product group: 0
@##Che4s6E@## -> product group: 46
Input
On the first line you will be given an integer n – the count of barcodes that you will be receiving next. 
On the next n lines, you will receive different strings.
Output
For each barcode that you process, you need to print a message.
If the barcode is invalid:
•	"Invalid barcode"
If the barcode is valid:
•	"Product group: {product group}"
Constraints

Examples
Input	Output
3
@#FreshFisH@#
@###Brea0D@###
@##Che4s6E@##	Product group: 00
Product group: 0
Product group: 46
Input	Output
6
@###Val1d1teM@###
@#ValidIteM@#
##InvaliDiteM##
@InvalidIteM@
@#Invalid_IteM@#
@#ValiditeM@#	Product group: 11
Product group: 00
Invalid barcode
Invalid barcode
Invalid barcode
Product group: 00


