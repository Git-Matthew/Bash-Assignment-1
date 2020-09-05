# Bash Examples 1
### Part 1: Commands

- **mkdir**

	**Description:** Creates a folder

	**Example:** mkdir my_dir

- **cd**

	**Description:** Takes you to a directory

	**Example:** cd my_dir

- **history**

	**Description:** Shows commands used

	**Example:** history

- **clear**

	**Description:** Clears screen

	**Example:** clear

- **ls**

	**Description:** Shows contents of a directory

	**Example:** ls

	**Parameters:**

	- **-l**: Shows contents in list format
	
	- **-A**: Show everything including hidden files
	
	- **-Al**: Show everything including hidden files in list format
	- **-Alh**: Show everything including hidden files in human list format

- **nano**

	**Description:** Open nano editor and create a file

	**Example:** nano file.txt

- **cat**

	**Description:** Shows contents of a file

	**Example:** cat file.txt

- **cp**

	**Description:** Copy a file

	**Example:** cp filein.txt fileout.txt

	**Parameters:**

	- **-i**: Interactive copying which can prompt for user selection
	
	- **-R**: Recursive copying which is used for directories

- **man**

	**Description:** Shows a manual on a specific command

	**Example:** man ls

- **rm**

	**Description:** Removes a file

	**Example:** rm file.txt

	**Parameters:**

	- **-R**: Recursively delte a directory

- **rmdir**

	**Description:** Removes an empty directory

	**Example:** rmdir my_dir1

- **mv**

	**Description:** Moves a file

	**Example:** file.txt /my_dir2

- **mv**

	**Description:** Rename a file

	**Example:** file.txt book.txt

- **pwd**

	**Description:** Shows working directory

	**Example:** pwd

- **locate**

	**Description:** Locates files and directories with a ceirtain word

	**Example:** locate spark

- **find**

	**Description:** Finds directories where files with that name exist

	**Example:** find . -name Minecraft

- **stat**

	**Description:** Shows statistics of a file such as size and changes

	**Example:** stat file.c

- **chmod**

	**Description:** Grant execution permissions to the user

	**Example:** chmod +x file_name

### Part 2: Find Command
	find . -executable -atime +1 -name "Installer[[:alnum:]]*"
	find / -empty -atime +365 -name "Note[[:digit:]]*.txt"
	find . -readable -name "Book[[:alnum:]]*.pdf"
	find / -name "[[:alnum:]]_Dataset[[:digit:]]*.csv"
	find /home -name "my_file[[:digit:]]*.exe" -atime +7 -executable
