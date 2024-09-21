
Every program run from the command line has three data streams connected to it that serves as communication channel with the external environment

Stream Name                               Description

Standard Input(STDIN)                Data fed into the program

Standard Output(STDOUT)         Output from the program(defaults to the terminal)

Standard Error(STDERR)              Error messages(defaults to terminal)


Piping using the Pipe operator(`|`) and redirection using the left and right angle brackets connect these streams between programs and files to accommodate a near infinite no of possible use cases.

### Redirecting to a new file

In the previous command examples the output was print into the screen.Thsi is convenient most of the time but we can use the right angle bracket operator to save the output to a file, to keep it for future reference or manipulation.

echo "test" > redirection.txt

If we redirected the output to a non existent file, the file will be created automatically.
If we redirected the output to an already existing file, the file contents will be replaced.

### Redirecting to an Existing file

To append additional data to an existing file as opposed to overwriting the file, we use the double right angled operator.

echo "test" >> redirection.txt

### Redirecting from a file

We can use the left angle bracket operator to send data the other way.

wc -m < redirection_test.txt

### Redirecting STDERR

According to the specifications , the file descriptors for STDIN, STDOUT, STDERR are defined as 0,1 and 2 respectively.

ls ./test.txt 2>error.txt




