
When opening a  terminal window a new bash process which has its own environment variables is initialized.

These variables are a form of global storage for various settings inherited by any applications that are run during that terminal session


PATH  Which is a colon separated list of directory paths that bash will search through whenever a command is run without a full path.

We can view the contents of a given environment variable with the echo command followed by the $ sign character and the environment variable name.

echo $PATH

Some other useful environment variable is USER, PWD and HOME

We can define an environment variable with the export variable

`export var_name="string"`

For eg when we are scanning a target and we don't want to type the IP address of the system repeatedly, we can quickly assign it as an environment variable and use that instead

The export command makes the variable accessible to any sub processes we might spawn from our current bash instances.If we set an environment variable without export, it will be available in the current shell.

To view all the variablee available in your linux system, we use the command `env`

