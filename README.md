# Lab 04

## Part 1: Standard Output Redirection

### Tasks
- Redirect the output of the `ls` command to a file named `files_list.txt`
- Display the contents of the `numbers.txt` file using the `cat` command, and redirect the output to a file named `numbers_copy.txt`
- Use the `echo` command to add a new line with the text "This is a new line" to the end of `numbers_copy.txt` file using the append operator
- Use the `ls` command with the `-la` option and redirect its output to the file `directory_info.txt`
- Create a file named `timestamp.txt` containing the current date and time by redirecting the output of the `date` command

## Part 2: Standard Error Redirection

### Tasks
- Attempt to list a non-existent directory and redirect the error message to a file called `errors.log`
- Run a command to find all files with `.txt` extension in your home directory, redirecting any errors to a file named `find_errors.log` and the successful output to `found_files.txt`
- Create a file that combines both standard output and standard error from the `grep` command when searching for the pattern "ERROR" in `server.log` (redirect to `all_output.log`)
- Try to read a file that doesn't exist and redirect the error to `/dev/null` (effectively silencing the error)
- Run a command that generates both output and errors, saving the output to `command_output.txt` and the errors to `command_errors.txt`

## Part 3: Pipes

### Tasks
- Count the number of lines in the `server.log` file using a pipe with `wc -l`
- List only files with the `.txt` extension in the current directory using a pipe with `grep`
- Display a sorted list of unique fruits from the `unsorted_data.txt` file using pipes
- Find all lines in `server.log` containing the word "ERROR" and count them using pipes
- Extract only the username field (first column) from `users.txt` and sort it alphabetically using pipes
- Count how many users belong to each department using pipes with `cut` and `sort` and `uniq -c`
- Find the top 3 largest files in the current directory using pipes
- List all log entries from `server.log` between 10:00 and 12:00 using `grep` and pipes

## Part 4: Here Documents

### Tasks
- Create a new file called `introduction.txt` using a here document with at least 3 lines of text
- Use a here document with the `grep` command to search for multiple patterns in `server.log`
- Create a simple HTML file named `simple.html` using a here document
- Use a here document with the `sed` command to perform multiple substitutions on `users.txt`
- Execute multiple SQL-like commands using a here document (simulate with `echo` or another command)

## Part 5: Here Strings

### Tasks
- Use a here string to count the number of characters in the text "Linux is an open-source operating system"
- Search for the word "apple" in a here string containing a list of fruits
- Convert a string to uppercase using a here string with the `tr` command
- Use a here string to check if a specific IP address is present in the `server.log` file
- Sort the comma-separated values "3,1,4,1,5,9,2,6" using a here string

## Part 6: Process Substitution

### Tasks
- Compare the contents of `dir1_files.txt` and `dir2_files.txt` using `diff` with process substitution
- Sort both `dir1_files.txt` and `dir2_files.txt` and find common files using `comm` with process substitution
- Use `paste` with process substitution to combine the sorted contents of `numbers.txt` with the uppercase version of the same file
- Find the differences between the original `unsorted_data.txt` and a sorted version using process substitution
- Create a backup of `users.txt` where all instances of "company.com" are replaced with "newcompany.com" using process substitution

## Part 7: Combining Techniques

### Tasks
- Create a report showing all ERROR and WARNING entries from `server.log`, sorted by time
- Extract all unique email addresses from `users.txt` and save them to a file called `emails.txt`
- Count the occurrences of each log level ([INFO], [ERROR], [WARNING]) in `server.log` and create a summary
- Find files that exist in `dir1_files.txt` but not in `dir2_files.txt` and vice versa
- Process `server.log` to create a list of users who logged in, along with their login times
