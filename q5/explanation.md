Q5: Storage Health Assessment — explanations

1. `lsblk` — listed block devices and partitions.
   Explanation: Shows available disks and their partitioning/mountpoints.

2. `mount | head` — displayed active mounts.
   Explanation: Identifies mounted filesystems and options.

3. `df -h` — provided human-readable disk usage.
   Explanation: Useful to assess free/used space before deployment.

4. `df -i` — provided inode utilization.
   Explanation: Checks for inode exhaustion which can block file creation even when space remains.

5. Created `Storage_Assessment_Report.txt` using the collected outputs and notes.
   Explanation: Prepared the required report file summarizing findings and recommendations.
