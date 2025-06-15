#alu-shell: Loops, Conditions, and Parsing Exercises
This repository contains a series of Bash scripting exercises focused on mastering loops, conditions, and text parsing in Linux environments. These exercises progress from simple tasks to more complex parsing and data processing, often working with system files and logs.

#Exercise Overview
1. 00-hello_world
Prints a simple "Hello World" message to the terminal.

2. 01-variables
Demonstrates how to create and use variables in Bash scripts.

3. 02-readme
Basic introduction to reading user input with read.

4. 03-for_loop
Uses a for loop to iterate over a list of items and display them.

5. 04-while_loop
Shows how to use a while loop to repeat actions until a condition is met.

6. 05-if_else
Introduces conditional statements (if-else) to control script flow.

7. 06-case_statement
Uses the case statement to handle multiple conditions more cleanly.

8. 07-parse_csv
Parses a CSV file using shell tools and prints formatted output.

9. 08-check_root
Checks if the script is run by the root user and acts accordingly.

10. 09-merge_files
Merges content from multiple files into one, demonstrating file manipulation.

11. 12-tell_the_story_of_passwd
Parses the /etc/passwd file using a while loop and IFS, then prints a formatted story about each user’s details.

12. 13-lets_parse_apache_logs
Extracts visitor IPs and HTTP status codes from an Apache access log, printing them in a simple IP HTTP_CODE format using awk.

13. 14-dig_the-data
Counts and groups visitor IPs with their HTTP status codes from Apache logs, displaying the number of occurrences sorted from highest to lowest. Uses awk and sort.

#How to Use
Clone this repository:

bash
Copy
Edit
git clone https://github.com/your-username/alu-shell.git
cd alu-shell/loops_conditions_and_parsing
Make the scripts executable (if not already):

bash
Copy
Edit
chmod +x *
Run each script as needed. For example:

bash
Copy
Edit
./12-tell_the_story_of_passwd
./13-lets_parse_apache_logs
./14-dig_the-data

#Notes
The scripts progressively introduce important Bash concepts and shell utilities.

For the Apache log exercises, ensure the apache-access.log file is present in the directory.

Some exercises require you to avoid using certain commands (for, while, sed, cut, etc.) to practice alternative approaches.

#License
This project is for educational purposes.