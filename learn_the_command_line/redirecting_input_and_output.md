### Redirection
- `stdin` standard input, information inputted into the terminal through the keyboard or input device.
    - `<` takes the standard input from the file on the right and inputs it into the program on the left. 
- `stdout` standard output, the information outputted after a process is run.
    - `>`  takes the standard output of the command on the left, and redirects it to the file on the right. 
    - `>>` add to a file without losing the original text
    - The `|` takes the standard output of the command on the left, and pipes it as standard input to the command on the right.
- `stderr`standard error, an error message outputted by a failed process.

- `sort` takes the standard input and orders it alphabetically for the standard output 

- `uniq` It filters out adjacent, duplicate lines in a file.


- `grep` global regular expression print
    - `-i`-i enables the command to be case insensitive
    - `grep -R` searches all files in a directory and outputs filenames and lines containing matched results. 
    - `grep -Rl` searches all files in a directory and outputs only filenames with matched results (so no lines)
    
- `sed` stands for “stream editor.” It accepts standard input and modifies it based on an expression, before displaying it as output data.
    - `sed 's/snow/rain/g' forests.txt`
    - The above command uses the g expression, meaning “global.”