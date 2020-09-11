# Bash Examples 1
### Part 1: Commands Class 1 & 2

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

### Part 3: Commands Class 3 & 4

- **head**

	**Description:** Shows the first n lines of a file (Default is 10)

	**Example:** head file.txt

	**Parameters:**

	- **-n**: Used to select how many lines it will show

- **tail **

	**Description:** Shows the last n lines of a file (Default is 10)

	**Example:** tail file.txt

	**Parameters:**

	- **-n**: Used to select how many lines it will show

- **wc**

	**Description:** Displays the number of lines/words/characters in a file

	**Example:** wc file.txt

	**Parameters:**

	- **-l**: Show number of lines
	- **-m**: Show number of characters
	- **-lm**: Show number of lines and characters

- **sort**

	**Description:** Organizes the lines in alphabetical order

	**Example:** sort file.txt

	**Parameters:**

	- **-n**: Organizes them numerically (Smallest to largest)
	- **-n -r**: Organizes them numerically in reverse (Largest to smallest)

- **column**

	**Description:** Replaces a separator from a file

	**Example:** column -s"\t" -t data.txt

	**Parameters:**

	- **-s**: Select a separator
	- **-t**: Select a file

- **shuf**

	**Description:**  Grabs a ceirtain number of random lines from a file

	**Example:** shuf -n 10 file.txt

	**Parameters:**

	- **-n**: number of lines

- **grep**

	**Description:** Looks for the lines which contain a word

	**Example:** grep "pizza" file.txt

	**Parameters:**

	- **-v**: Display the lines without a pattern

- **touch**

	**Description:** Create an empty file or turn one into an empty file

	**Example:** touch file.txt


- **cut**

	**Description:** Cut the defined element in the assigned delimitation (character) from a file.

	**Example:** cut -d"." -f1 file.txt

	**Parameters:**

	- **-f**: Acts as a limiter 

- **echo**

	**Description:** Writes down into a file

	**Example:** echo "stuff" > file.txt

- **variables**

	**Description:** Creates variables

	**Example:** variable="Stuff"

### Part 4: Path
	 cat file.txt | head
	 echo > "String Stuff And More Stuff" file.txt | wc
	 tail file.txt | shuf -n 10
	 echo "Things To Write" > file.txt | touch file.txt | echo "Cleaned"
	 sort -nr file.txt | grep "stuff"
