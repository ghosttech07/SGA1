Q3: File System and Link Analysis — explanations

1. `echo "Linux link test file" > original.txt` — created the test file.
   Explanation: Prepared a file to experiment with links.

2. `ln original.txt hardlink.txt` — created a hard link.
   Explanation: Hard link creates an additional directory entry referring to same inode.

3. `ln -s original.txt symlink.txt` — created a symbolic link.
   Explanation: Symlink stores a pathname that points to the target file.

4. `ls -li` / `stat` — observed inode numbers and link counts.
   Explanation: Confirmed hard link shares inode; symlink has its own inode and points to the name.

5. `rm original.txt` — removed the original path.
   Explanation: Hard link still provided access to data; symlink became broken because it referenced the removed pathname.
