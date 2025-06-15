#Processes and Signals – ALU Shell Project
This folder contains a collection of Bash scripts that help you understand how to manage processes in Linux. Each script introduces a small but important concept like getting your process ID (PID), handling signals, and even creating a basic process manager.

# Scripts Breakdown
0-what-is-my-pid
Prints the PID (Process ID) of the script itself using $$.

1-list_your_processes
Shows a list of your running processes using the ps command.

2-show_your_bash_pid
Displays the PID of your current Bash shell using pgrep.

3-show_your_bash_pid_made_easy
An even simpler way to get your Bash PID using pidof.

4-to_infinity_and_beyond
Prints “To infinity and beyond” forever, once every second. A simple infinite loop!

5-dont_stop_me_now
Stops the infinite script above (4-to_infinity_and_beyond) by killing it.

6-stop_me_if_you_can
Does the same thing as 5-dont_stop_me_now, but uses a different method to stop the process — without using kill or killall.

7-highlander
Runs an infinite loop printing “To infinity and beyond” every 2 seconds.
If it receives a SIGTERM signal, it prints: I am invincible!!!

67-stop_me_if_you_can
This script finds the 7-highlander process and triggers the signal that makes it print I am invincible!!!.

8-beheaded_process
This one goes all the way—kills the 7-highlander process entirely using the kill command.

10-process_and_pid_file
Creates a PID file at /var/run/myscript.pid and reacts to different signals:

SIGTERM → “I hate the kill command”

SIGINT (Ctrl+C) → “Y U no love me?!”

SIGQUIT → Cleans up and stops

It also prints “To infinity and beyond” continuously like before.

manage_my_process
A small background process that prints “I am alive!” to the file /tmp/my_process every 2 seconds.

11-manage_my_process
A mini init-style script that lets you manage manage_my_process:

start → Launches the process and saves its PID to /var/run/my_process.pid

stop → Stops the process and deletes the PID file

restart → Does both stop and start

Any other input → Shows: Usage: manage_my_process {start|stop|restart}

# How to Test These Scripts
You’ll often need to run them in two terminals:

Terminal #1 to start the process

Terminal #2 to stop, restart, or interact with it

Some scripts (like 10-process_and_pid_file or 11-manage_my_process) may need sudo since they write to /var/run.

