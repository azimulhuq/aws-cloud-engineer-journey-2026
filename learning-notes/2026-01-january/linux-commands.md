# Linux Commands

## File & Directory Management
**ls - List Directory Contents**
- ls                        # List files and directories
- ls -la                    # List all files (including hidden) with details
- ls -lh                    # List with human-readable file sizes
- ls -lt                    # List sorted by modification time
- ls -R                     # List recursively (subdirectories)
- ls *.txt                  # List only .txt files

**cd - Change Directory**
- cd ~                      # Go to home directory
- cd -                      # Go to previous directory
- cd ..                     # Go to parent directory
- cd ~/path/to/dir          # Go to specific directory

**pwd - Print Working Directory**
- pwd                       # Show current directory path

**mkdir - Make Directory**
- mkdir dirname             # Create a directory
- mkdir -p dir1/dir2        # Create nested directories
- mkdir -m 755 dirname      # Create with specific permissions

**touch - Create Empty File**
- touch filename            # Create empty file
- touch file1 file2         # Create multiple files

**cp - Copy Files and Directories**
- cp file1 file2            # Copy file1 to file2
- cp -r dir1 dir2           # Copy directory recursively
- cp -p file1 file2         # Preserve permissions and timestamps
- cp -i file1 file2         # Interactive copy (prompt before overwrite)

**mv - Move/Rename Files**
- mv file1 file2            # Rename file1 to file2
- mv file1 /path/dir        # Move file1 to directory
- mv -i file1 file2         # Interactive move

**rm - Remove Files**
- rm filename               # Remove file
- rm -r dirname             # Remove directory recursively
- rm -f filename            # Force remove (no confirmation)
- rm -rf filename           # Force Remove directory recursively (no confirmation)
- rm -i filename            # Interactive remove

**find - Find Files**
- find . -name "*.txt"      # Find .txt files in current directory
- find /home -user username # Find files owned by user
- find . -size +100M        # Find files larger than 100MB
- find . -mtime -7          # Find files modified in last 7 days

**rmdir - Remove Directory**
- rmdir dirname             # Remove empty directory
- rmdir -p dir1/dir2        # Remove directory and parent if empty

## File Content Manipulation
**cat - Concatenate and Display Files**
- cat filename              # Display file content
- cat file1 file2           # Display multiple files
- cat > filename            # Create file with input
- cat >> filename           # Append to file

**tac - Reverse Cat**
- tac filename              # Display file content in reverse order

**head - Display Beginning of File**
- head filename             # Display first 10 lines
- head -n 20 filename       # Display first 20 lines
- head -c 100 filename      # Display first 100 characters

**tail - Display End of File**
- tail filename             # Display last 10 lines
- tail -n 20 filename       # Display last 20 lines
- tail -c 100 filename      # Display last 100 characters

**less - Advanced File Viewer**
- less filename             # Display file with navigation
- less -N filename          # Display with line numbers

**grep - Search Text**
- grep "pattern" file.txt           # Search for pattern
- grep -i "pattern" file.txt        # Case-insensitive search
- grep -r "pattern" directory/      # Recursive search
- grep -v "pattern" file.txt        # Invert match
- grep -n "pattern" file.txt        # Show line numbers