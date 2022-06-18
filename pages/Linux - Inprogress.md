- #+BEGIN_IMPORTANT
  Linux commands are case sensitive
  #+END_IMPORTANT
- Basic commands
	- `echo hello`
	- ```bash
	  echo hello
	  #hello
	  
	  echo hello world
	  #hello world
	  
	  echo -n hello
	  #hello
	  ```
	- `man`
	  collapsed:: true
		- > To get manual page
		- ![image.png](../assets/image_1655573854145_0.png)
		- Anything within `[]` brackets are optional
		- > `F` to scroll one page `B` to scroll backpage
		- > `/` <<search word>> to search any. `N` to find the next match
		-
		-
	- Help
		- > `man --help` or `man -h` or `man - ?` to find the help
	- File
		- Create new file
			- `touch <<filename`
		- To read the file
			- `cat <<filename>>`
		- Pass output of cmd to a file
			- `echo "hi" > <<filename>>` -> This replace all the contents in a file
			- `echo "hi" >> <<filename>>` -> This adds text to the end of the file
		- Copy the file
			- `cp <<filename>> <<destination>>`
		- Move the file
			- `mv <<filename>> <<destination>>`
	- Directories
	  collapsed:: true
		- `pwd` -> To know the current working directory
		- Create directory
			- `mkdir <<directory name` -> creates a directory
		- Delete the directory and files init
			- `rm -r <<directory name>>` -> Deletes the directory and files within it
			- To delete just the directory
				- `rm -d <<directory name`
	- Variables
		- Set variable value `test_var=Hi`
		- To refer variables use $ `echo $test_var`
		-
	-
		-
	-