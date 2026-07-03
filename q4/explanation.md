Q4: File Access and I/O Investigation — explanations

1. `echo "sample log line" > app.log` — created an application log file.
   Explanation: Provides a file to open and inspect descriptors.

2. `lsof` — listed system-wide open files; used `lsof -p $$` to focus on the current shell.
   Explanation: Identifies open file descriptors held by processes.

3. `exec 3<app.log` — opened `app.log` on file descriptor 3 for reading.
   Explanation: Demonstrates manual file descriptor assignment and persistence while open.

4. `ls -l /proc/$$/fd` and `ls -l /proc/$$/fd | grep app.log` — showed descriptor 3 links to `app.log`.
   Explanation: Confirms mapping between fd and filesystem path.

5. `ls -l > stdout.txt`, `ls /not_a_real_path 2> stderr.txt`, `(ls -l && ls /not_a_real_path) > combined.txt 2>&1` — demonstrated redirection behaviors.
   Explanation: Shows separation and combining of stdout/stderr streams.

6. `ulimit -a` — displayed resource limits.
   Explanation: Useful to detect constraints impacting file I/O.
