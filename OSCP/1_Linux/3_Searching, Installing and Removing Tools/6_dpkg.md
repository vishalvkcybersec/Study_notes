
dpkg is the core tool used to install a package either directly or indirectly through apt.

It is also the preferred tool to use when operating offline since this doesn't require an internet connection.

The dpkg doesn't install any dependencies that a package might require. To install the package, provide the -i option and the path to the package file.

Syntax : `dpkg -i file_path /file`