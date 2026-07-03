Q1: Environment Verification — explanations

1. `whoami` — showed the current user `codespace`.
   Explanation: Identifies the account used to run lab commands.

2. `groups` — listed group memberships.
   Explanation: Shows supplementary group access for the account.

3. `echo "$SHELL"` — printed `/bin/bash`.
   Explanation: Confirms the user's login shell.

4. `pwd` — printed `/`.
   Explanation: Confirms the working directory when the commands were run.

5. `ls -ls` — produced the root directory listing (captured in screenshots).
   Explanation: Lists files and directories present in the workspace/root.

6. `curl -s --max-time 10 https://youtube.com` — network reachable.
   Explanation: Verifies outbound network connectivity to the test site.
