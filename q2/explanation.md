Q2: Secure Project Workspace Setup — explanations

1. `mkdir -p secure_workspace/{docs,src,logs}` — created project directories.
   Explanation: Sets up a structured workspace for documentation, source, and logs.

2. `touch ...` — created `plan.txt`, `app.txt`, and `activity.log`.
   Explanation: Provides placeholder files for documentation, code, and logging.

3. `ls -ld secure_workspace secure_workspace/*` — listed directories and initial permissions.
   Explanation: Used to verify creation and current permission bits.

4. `chmod 750 ...` — set directory permissions to `rwxr-x---`.
   Explanation: Restricts access to owner and group while denying others.

5. `chmod 640 ...` — intended to set file permissions to `rw-r-----`; `activity` typo caused one file to remain world-writable.
   Explanation: Shows importance of correct file names when applying permissions.

6. `umask` — printed `0022`.
   Explanation: Indicates default permission mask used when creating new files.
