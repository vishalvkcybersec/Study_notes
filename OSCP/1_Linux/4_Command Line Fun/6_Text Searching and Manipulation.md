
### Grep
The grep command searches text files for the occurrence of a given regular expression and output any line that contains a match to the STDOUT.

`ls -la /usr/bin | grep zip`

Some of the commonly used switches for the grep command is

-r  for recursive searching
-i to ignore the case of the search term


### sed
sed is a powerful stream editor. sed performs text editor on a stream of text, either a set of specific files or STDOUT.


`echo "I need to try hard" | sed 's/hard/harder/'`


### cut
The cut command is used to extract a section of text from a line and output it to STDOUT.

Some of the commonly used switches include 
-f for field number we are cutting
-d to define the field delimiter

`echo "I hack binaries,web apps,mobile apps, and just about anything else" | cut -f 2 -d ","`

The output is      
web apps

The below command  provides the first field that is the list of all the user from the /etc/passwd file

`cut -d ":" -f 1 /etc/passwd`

### awk
awk is a programming language designed for text processing and is typically used for data extraction and reporting tool. 

The commonly used switch with the awk command is

-F   field separator
print command which outputs the result text

`echo "hello::there::friend" | awk -F "::" '{print $1, $3}'`

Here we echoed a line and piped it to awk to extract the first and third field using the ':' as a field separator

cut can only except a single character as a field delimiter while awk is much more flexible
